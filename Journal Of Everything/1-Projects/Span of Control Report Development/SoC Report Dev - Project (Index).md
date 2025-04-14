# Span of Control Reporting Development

See 
	`OneDrive/Documents/projects/supervisor_reports/main.py
	`OneDrive/environments/supervisor_reports`
## Project Overview
- **Status**: Active
- **Start Date**: 2025-03-31
- **Target Completion Date**: 2025-04-08
- **Project Lead**: Caroline Cote
- **Project Members**: Ian Johnson, Caroline Cote
- **Project Directory**:  [Supervisor_Reports](file:////C:/Users/ijohnson/OneDrive%20-%20University%20of%20Vermont/Documents/projects/supervisor_reports) 
## Project Purpose
Produce supervisor span of control (direct reports) reporting that can provide high level summary data and detailed information about network connections in the organization. 

These reports are intended to be used by the President and CHRO.
## Key Documents

[[SoC Report Dev - Analysis Groupings]] - High level groupings to use when examining summary statistics such as totals and averages.
[[SoC Report Dev - Deliverables]] - The expected output upon project completion
[[Graph Network Analysis Resource]] - General information about graph networks, theory and code.
## Project Timeline

- [x] 2025-03-31: Initial Request from Caroline
- [x] 2025-04-01: Graph network analysis developed in Python script.
- [x] 2025-04-03: Initial network data review with Caroline
- [ ] 2025-04-08: Summarized data draft for review with Caroline
- [ ] 

## Project Notes
- Initially attempted class based Employee/Supervisor linked object/dictionaries/lists route. 
	- Became increasingly complex and unwieldy as more data and attributes were added.
	- Significantly Slower.
	- Harder to extend to network based theorieas.
- Data cleanup idenfied
	- Orphaned supervisors and employees with no active supervisor id or supervisor posn
	- Comparison of supervisor and manager CPD stream and level require further analysis
- 