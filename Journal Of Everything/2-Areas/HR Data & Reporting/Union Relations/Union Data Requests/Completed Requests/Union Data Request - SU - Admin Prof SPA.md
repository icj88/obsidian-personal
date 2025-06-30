# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	-  June 4, 2025
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
		- Not quite. Requests full Job Descriptions
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [x] Customize main.R script in union_data_requests R Project
- [x] Pull Data
- [x] Run R Script
- [x] Verify data accuracy/formatting
- [x] Format xlsx output
- [x] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request
> Good morning, 
> 
> I sent the previous information request too early and a second one was sent afterwards. Can you please add “Sr. Research Administrator” to the report as well?
> 
> Thank you!
> 
> Best,
> Amanda
> 
> From: Diana Naser <Diana.Naser@uvm.edu> 
> Sent: Tuesday, May 20, 2025 4:37 PM
> To: HR Partners <HRPartners@uvm.edu>; Amanda Desmond <Amanda.Desmond@uvm.edu>
> Cc: Elizabeth Dunford (she/her) <Elizabeth.Dunford@uvm.edu>; Jack Roberts <Jack.Roberts@uvm.edu>; Diana Naser <Diana.Naser@uvm.edu>
> Subject: RE: Information Request
> 
> Hi Amanda, 
>  
> With the knowledge and approval of UVMSU, I am writing to request the job descriptions for UVMSU Cluster #9, Sponsored Project Administration, that have “Administrative Professional”, “Research Administrator”, or “Sr. Research Administrator” as either the Position Title or Working/Business Title. 
> 
> Thanks 
> Diana
> 
> Hi there, 
> 
> Please see the information request below from UVMSU. Diana references Cluster #9, but I believe she’s looking for all employees in SPA with the “Administrative Professional” and/or “Research Administrator” titles.
> 
> Best,
> Amanda
> 
> From: Diana Naser <Diana.Naser@uvm.edu> 
> Sent: Tuesday, May 20, 2025 4:27 PM
> To: HR Partners <HRPartners@uvm.edu>; Amanda Desmond <Amanda.Desmond@uvm.edu>
> Cc: Jack Roberts <Jack.Roberts@uvm.edu>; Elizabeth Dunford (she/her) <Elizabeth.Dunford@uvm.edu>; Diana Naser <Diana.Naser@uvm.edu>
> Subject: Information Request
> 
> Hi Amanda, 
> 
> With the knowledge and approval of UVMSU, I am writing to request information about how salaries were determined for the following individuals in their current positions: All employees in UVMSU Cluster #9, Sponsored Project Administration, with the job titles “Administrative Professional” and/or “Research Administrator.” 
> 
> Please include information about:                                                                                                               
> -	Years of UVM experience
> -	Years of non-UVM experience
> -	Education
> -	Hire date
> -	FTE
> -	Term
> -	Job Classification
> -	Minimum salary for the pay range
> -	Maximum salary for the pay range
> -	The percentile in which the individual falls in that current range
> -	Current Hourly Rate (actual)
> -	Current annual salary rate (actual)
> -	Current annual salary rate adjusted for shift differential
> -	Current annual salary rate adjusted for FTE and Term
> -	Salary justification (means and evidence for determining salary including complexity of role)
> -	Level of complexity (numeric value)
> -	Any other materials relevant to determining salary placement
> 
> Thank you,
> Diana


## Original

> Quoted Original Email from the original requestor (if not in the primary request section)

# Datasets and Sources
- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_ICJ_JOBCODETBL_ALL [Salary/Wage Band Min/Max]
- [x] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....

# Notes
General [[Union Data Request Notes]]
[[Union Data Requests  - Position Descriptions]]

# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *<file_name>.xlsx*
Script File Name:    *<script_file_name>.R* 

Response Email Date:       *2025-05-21*
Response Email Subject:   *RE: Information Request
