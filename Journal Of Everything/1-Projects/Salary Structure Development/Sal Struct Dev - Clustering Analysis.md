# Natural Salary Clustering Analysis

A natural salary clustering analysis helps id where salaries naturally group together, to help inform how many distinct salary bands we need.
## **Data Collection and Preparation**
- Gather all current salary data for UVM
- Include job information (family, sub-family, career type, level)
- Clean the data (remove outliers, handle missing values)
- Normalize salaries if comparing across regions with different cost-of-living factors
## **Initial Data Visualization**
- Create scatter plots of salaries across UVM
- Plot histograms to see the overall distribution
- Develop box plots by job family, career type, and level
- Look for natural breakpoints where salaries visibly cluster
## **Statistical Clustering Analysis**
- Apply k-means clustering algorithm with different values of k (clusters)
- Try hierarchical clustering to visualize potential groupings
- Use silhouette analysis to evaluate the quality of clusters
- Test different combinations of variables (salary, experience, level)
## **Interpretation and Validation**
- Review the clusters against the CPD architecture
- Check if clusters align with the CPD job families and levels
- Validate whether the clusters make intuitive sense
- Identify where clusters cross job families (potential for consolidated bands)
## **Refinement and Testing**
- Adjust cluster parameters based on organizational context
- Test sensitivity by adding/removing data points
- Compare against existing or planned career pathways
- Analyze the stability of clusters with simulated salary changes
## **Example Analysis Process**
1. **Initial Exploration:** Plot all salaries on a single axis and look for natural breaks or multi-modal distributions
2. **Depth Analysis:** Calculate the salary frequency distribution and identify peaks and valleys that might indicate natural band boundaries
3. **Family-Level Analysis:** Perform separate clustering for each job family to see if different families have different natural clustering patterns
4. **Validation Check:** For each potential cluster boundary, analyze what percentage of employees would fall into unusual positions relative to their job level
## **Example Findings**
Look for patterns, for example:
- Five distinct salary clusters that align well with the five cpd levels
- Some job families showing compression (fewer natural clusters than levels)
- Others showing expansion (more natural clusters than formal levels)
- Potential need for different band structures across different job families

This analysis helps ensure the band structure reflects the actual salary landscape rather than imposing an artificial structure that doesn't match how compensation actually works at UVM