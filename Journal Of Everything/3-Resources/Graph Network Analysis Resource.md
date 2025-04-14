# Basic Graph Theory Concepts


# Graph Specific Metrics
### Influence Score (Degree Centrality)

**Technical definition:** A network measure of how connected a person is to others in the organization.

**Non-technical explanation:** "This score indicates how connected someone is within the organization. People with high influence scores interact with or affect many other employees directly.

Think of it as measuring someone's 'reach' in the organization. A person with high influence might not necessarily be high in the hierarchy, but they have connections to many parts of the organization. For example, an executive assistant who works with multiple departments or a systems administrator who supports many teams might have a surprisingly high influence score because of their numerous direct connections."

### Bottleneck Score (Betweenness Centrality)

**Technical definition:** Measures how often a person lies on the shortest path between other pairs of individuals in the network.

**Non-technical explanation:** "This score identifies people who serve as bridges between different parts of the organization. Someone with a high bottleneck score is like a crucial intersection in a road network - a lot of information, decisions, or workflows have to pass through them.

For example, if Alice is the only person who regularly communicates between the Marketing and Engineering departments, she would have a high bottleneck score. If she's absent, communication between these departments might break down. This metric helps identify potential vulnerable points in your organization where information flow depends heavily on specific individuals."


# NetworkX Coding Patterns
See [NetworkX Python Documentation Site](https://networkx.org/documentation/stable/) r
## Build  graph, assign nodes and relations
```python 
# Create a directed graph
    G = nx.DiGraph()
    data = df.copy()
    
    # Add employees as nodes
    employees = data[['emplid', 'name_full_legal', 'fscm_rollup', 'dept_desc',
                      'job_title_working', 'jobcode_desc', 'empl_type', 'is_primary', 'supv_id']].drop_duplicates()
    
    all_employees = data[['emplid', 'name_full_legal', 'fscm_rollup', 'dept_desc',
                          'job_title_working', 'jobcode_desc', 'empl_type', 'is_primary', 'supv_id']].copy()
    
    # Get a list of all unique employee IDs
    all_emplids = all_employees['emplid'].unique()
    
    # Get all supervisor IDs that might not be in our employee list
    all_supv_ids = data['supv_id'].dropna().unique()
    
    # Find missing supervisor IDs
    missing_supv_ids = set(all_supv_ids) - set(all_emplids)
    
    # For primary job records, prioritize those
    primary_employees = all_employees[all_employees['is_primary']].drop_duplicates(subset=['emplid'])
    
    # For employees without primary jobs, take their first record
    non_primary_employees = all_employees[~all_employees['emplid'].isin(primary_employees['emplid'])].drop_duplicates(subset=['emplid'])
    
    # Combine the dataframes to get one record per employee
    unique_employees = pd.concat([primary_employees, non_primary_employees])
    
    for _, row in unique_employees.iterrows():
        G.add_node(row['emplid'],
                   name=row['name_full_legal'],
                   title=row['job_title_working'],
                   jobcode_desc=row['jobcode_desc'],
                   fscm_rollup=row['fscm_rollup'],
                   department=row['dept_desc'],
                   emp_type=row['empl_type'])
        
    # Also add any missing supervisor IDs as placeholder nodes
    for supv_id in missing_supv_ids:
        if supv_id not in {"Vacant", "Vacant/NPC", None} and not pd.isna(supv_id):
            G.add_node(supv_id,
                       name=f"Unknown Supervisor ({supv_id})",
                       title="Unknown",
                       jobcode_desc="Unknown",
                       fscm_rollup="Unknown",
                       department="Unknown",
                       emp_type="unknown")
        
    # Add unique reporting relationships as edges
    relations = employees[['supv_id', 'emplid']].drop_duplicates()
    for _, row in relations.iterrows():

        if pd.notna(row['supv_id']) and not row['supv_id'] in {"Vacant", "Vacant/NPC"}:
            G.add_edge(row['supv_id'], row['emplid'])
            
    return G
```
# Organizational Network Metrics
# Visualization Approaches