# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	- July 14, 2025
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
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
> From: Amanda Desmond <Amanda.Desmond@uvm.edu> 
> Sent: Monday, June 30, 2025 10:24
> To: Rafae Khan <Rafae.Khan@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
> Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>
> Subject: FW: Equity Review Initiation 
> 
> Good morning,
> 
> Please see the requested information for all Administrative Professionals - Financial Analysts in Sponsored Project Admin below.
> 
> Thank you!
> Amanda

------

> From: Elizabeth Dunford (she/her) <Elizabeth.Dunford@uvm.edu> 
> Sent: Friday, June 27, 2025 9:19 AM
> To: HR Partners <HRPartners@uvm.edu>
> Cc: Jack Roberts <Jack.Roberts@uvm.edu>
> Subject: Equity Review Initiation 
> 
> Good morning,
> With the knowledge and support of UVMSU, I am requesting an equity review for all Administrative Professionals - Financial Analysts in Sponsored Project Admin, per Article 23.4.2 and Article 23.4.3 as agreed upon in the current UVMSU contract.
> We believe there is an equity issue because Heather Bullett brought to our attention that although she has over 20 years of relevant experience working both outside of UVM and in benefit service years at UVM, as well as having a non-terminal Master’s Degree, she is still being paid at a lower rate than individuals in the same job position (Financial Analyst) who either have comparable experience and education or less experience and education.
> After review, please provide documentation of the following items for each individual:
> •	Years of UVM experience
> •	Years of non-UVM experience
> •	Education
> •	Hire date
> •	FTE
> •	Term
> •	Job Standard
> •	Minimum salary for the pay range
> •	Maximum salary for the pay range
> •	The percentile in which the individual falls in that current range
> •	Current Hourly Rate (actual)
> •	Current annual salary rate (actual)
> •	Current annual salary rate adjusted for shift differential
> •	Current annual salary rate adjusted for FTE and Term
> •	Proposed annual salary (actual) after equity review
> •	Percent increase (if proposed) between current annual salary rate (actual) and proposed annual salary (actual) after equity review
> •	Salary justification (means and evidence for determining salary including complexity of role)
> •	Level of complexity (numeric value)
> •	Any other materials relevant to determining salary placement
> 
> Best,
> 
> Elizabeth Dunford

# Datasets and Sources
- [ ] UV_ACTIVE_EMPLS [General EE Info]
- [ ] UV_HR_HERD_SURVEY2 [Education]
- [ ] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [ ] UV_ICJ_JOBCODETBL_ALL [Salary/Wage Band Min/Max]
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
