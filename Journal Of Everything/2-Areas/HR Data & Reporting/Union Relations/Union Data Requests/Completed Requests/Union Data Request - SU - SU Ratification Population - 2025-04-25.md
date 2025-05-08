***Payroll to supply this dataset per Rafae Khan, Penny Cayia***
# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
		- [?] **Get Feedback on Personal Email and Phone Numbers**
		- Personal Email and phone numbers from SELRA reports
	- [x] Does the requestor have authority for the request?
		- **YES - Matthew Casey**
	- [x] Is the request satisfied using the standard template?
		- **NO**
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
	- **PeopleSoft, Possibly Payroll
	- 4/14 Pre wage change dataset supplied by Penny
	- [?] Do we need to Determine/Align Population with that used by PR, will we be supplying that?
	- UV_PAYROLL report for grant status
- [x] Customize *main.R* script in *union_data_requests* R Project
- [x] Pull Data
- [x] Run R Script
- [x] Verify data accuracy/formatting
- [x] Format xlsx output
- [x] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

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
		- [!] Use The benefit service date
> •	Date of hire into current position
		- [!] Position Entry Date
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
**Contact Info:**
- [x] [[PS - SELRA Report]] to determine the Allowed Information
**Job/Employee Info:**
- [x] UV_ACTIVE_EMPLS [General EE Info]
**Grant Funding:**
UVM Reports -> Commitment Funding -> Labor Distribution
# Notes
General [[Union Data Request Notes]]
See Student Researcher Project for Grant Funding Details

**Terminated Employees must be kept in file. ** Manually pull information for these employees if necessary. 
# Response
Compiled via newly created *union_data_requests* R Project. 

Output File Name:  *DataRequest_SU_All_PreRaise_20240505.xlsx*
Script File Name:    *20250414_su_ratification.R* 

Response Email Date:       *2025-05-07*
Response Email Subject:   *RE: UVMSU Contract Implementation & Payroll Coordination*
