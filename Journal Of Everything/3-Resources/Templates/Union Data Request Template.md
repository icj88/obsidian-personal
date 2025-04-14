# Data Request Checklist
- [ ] Determine response Deadline (typically, 10 business days)
- [ ] Review request 
	- [ ] Are the requested fields available?
	- [ ] Are the requested fields shareable?
	- [ ] Does the requestor have authority for the request?
	- [ ] Is the request satisfied using the standard template?
- [ ] Provide initial follow-up to business partner or requestor (if received directly)
- [ ] Create Entry in Obsidian [[Union Data Request Index]]
- [ ] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [ ] Customize main.R script in union_data_requests R Project
- [ ] Pull Data
- [ ] Run R Script
- [ ] Verify data accuracy/formatting
- [ ] Format xlsx output
- [ ] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [ ] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request

> Quoted Email Request and any relevant follow-ups here

## Original

> Quoted Original Email from the original requestor (if not in the primary request section)

# Datasets and Sources
- [ ] UV_ACTIVE_EMPLS [General EE Info]
- [ ] UV_HR_HERD_SURVEY2 [Education]
- [ ] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [ ] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [ ] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....

# Notes
General [[Union Data Request Notes]]


# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *<file_name>.xlsx*
Script File Name:    *<script_file_name>.R* 

Response Email Date:       *<YYYY-MM-DD\>*
Response Email Subject:   *RE: <Email Subject Line\>*
