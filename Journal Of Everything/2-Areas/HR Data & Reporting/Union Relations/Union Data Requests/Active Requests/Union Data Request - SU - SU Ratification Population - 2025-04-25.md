# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
- [ ] Review request 
	- [x] Are the requested fields available?
	- [ ] Are the requested fields shareable?
		- [?] **Get Feedback on Personal Email and Phone Numbers**
	- [x] Does the requestor have authority for the request?
		- **YES - Matthew Casey**
	- [x] Is the request satisfied using the standard template?
		- **NO**
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [ ] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
	- **PeopleSoft, Possibly Payroll
	- [?] Do we need to Determine/Align Population with that used by PR, will we be supplying that?
- [ ] Customize *main.R* script in *union_data_requests* R Project
- [ ] Pull Data
- [ ] Run R Script
- [ ] Verify data accuracy/formatting
- [ ] Format xlsx output
- [ ] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [ ] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request

> Good afternoon,
> 
> We received the following information request from UVMSU. Please let me know if you have any questions. Thanks!
> To help with the Payroll implementation across the board, please share as an info request a full list of staff in our bargaining unit as of 4/14/25 (date of ratification). The list should include:
> •	Employee ID
> •	Lived First Name
> •	Lived Last Name
> •	Home Address
> •	Mailing Address (if different)
> •	Home phone
> •	Work phone
> •	Cell phone
> •	Work email
> •	Personal email
> •	Department
> •	Job Code
> •	Job title
> •	Employee Class (9, 10, 11, 12 month appointment, etc.)
> •	FTE
> •	Standard Hours
> •	Date of hire at UVM
> •	Date of hire into current position
> •	(for non-exempt) Hourly wage before 4% raise
> •	(for exempt) Annual salary before 4% raise
> •	Indicate whether fully grant-funded, partially grant-funded, or non-grant-funded position.
> •	Supervisor Empl ID
> •	Supervisor Name
> 
> 
> Matthew Casey (he/him/his)
> HR Partner
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
Compiled via newly created *union_data_requests* R Project. 

Output File Name:  *<file_name>.xlsx*
Script File Name:    *<script_file_name>.R* 

Response Email Date:       *<YYYY-MM-DD\>*
Response Email Subject:   *RE: <Email Subject Line\>*
