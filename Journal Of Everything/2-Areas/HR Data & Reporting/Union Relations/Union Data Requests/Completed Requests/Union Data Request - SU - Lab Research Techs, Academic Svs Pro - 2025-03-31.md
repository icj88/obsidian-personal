# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
      2025-04-14
- [ ] Review request 
	- [x] Are the requested fields available?
	      New request item *Level of complexity (numeric value)* not available
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [x] Customize main.R script in union_data_requests R Project
- [x] Pull Data
- [x] Run R Script
- [x] Verify data accuracy/formatting
- [x] Format xlsx output
- [ ] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request

> Hello HR Partners,
>  
> With the knowledge and support of UVMSU, I am requesting information about how salaries were determined for the following employees per Article 23.9c as written in the side letter agreement signed on January 11, 2024:
>  
> -	Erin O'Neill - Academic Srvcs Professional 
> -	Maya Vaccaro - Lab/Research Technician 
> -	Alanis Papoulias - Lab/Research Technician 
> -	Kaitlyn Zoller - Lab/Research Technician 
>  
> Please provide documentation of the following items for each individual:
>  
> -	Years of UVM experience
> -	Years of non-UVM experience
> -	Education
> -	Hire date
> -	FTE
> -	Term
> -	Job Standard
> -	Minimum salary for the pay range
> -	Maximum salary for the pay range
> -	The percentile in which the individual falls in that current range
> -	Current Hourly Rate (actual)
> -	Current annual salary rate (actual)
> -	Current annual salary rate adjusted for shift differential
> -	Current annual salary rate adjusted for FTE and Term
> -	Proposed annual salary (actual) after equity review
> -	Percent increase (if proposed) between current annual salary rate (actual) and proposed annual salary (actual) after equity review
> -	Salary justification (means and evidence for determining salary including complexity of role)
> -	Level of complexity (numeric value)
> -	Any other materials relevant to determining salary placement
>  
> Sincerely,
> Andrew May
> UVMSU Area Steward

## Original

> Quoted Original Email from the original requestor (if not in the primary request section)

# Datasets and Sources
- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [x] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [x] Any others by request?
# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *DataRequest_ONeillVaccaroPapouliasZoller_20250409.xlsx*
Script File Name:    *20250409_ONeillVaccaroPapouliasZoller.R* 

Response Email Date:       *2025-04-09*
Response Email Subject:   *RE: Information Request
