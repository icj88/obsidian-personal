# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	- 2025-04-10 -> 2025-04-24
- [x] Review request 
	- [x] Are the requested fields available?
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
- [x] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request

> From: Jack Roberts <Jack.Roberts@uvm.edu>
> Sent: Thursday, April 10, 2025 1:47 PM
> To: HR Partners <HRPartners@uvm.edu>
> Cc: Matte Brittenham-Jones (they/them) <mbritten@uvm.edu>; Janelle Iris Seibert (she/her) <Janelle.Seibert@uvm.edu>
> Subject: Information Request: CHWB Healthcare Counselor Senior 
>  
> To whom this may concern:
>  
> On behalf of UVMSU, I am submitting an information request for the following:
> 	1) What is the current status and future plans for the Health Care Counselor Senior UVMSU bargaining unit position in the Center of Health and Wellbeing that was previously held by Jessica Ley Metcalf? 
> 		-  Does the department plan to hire someone to fill the position?
> 		- Does the department plan to eliminate the position?
> 		- Does the department plan to reduce the FTE of the position?
> 		- Is the CAPS Training Manager position that holds Jessica currently intended to cause the elimination of the Health Care Counselor Senior position or reduce that position’s FTE? 
> 	2) If the Health Care Counselor Senior position will be eliminated:
> 		- Will the work that was performed by Jessica in that role be eliminated completely? Or will the scope of her work be transferred to other employees?
> 		- Will any of the scope of that work be transferred to the CAPS Training Manager position that Jessica currently holds?
> 		- If yes, are those other employees bargaining unit members or non-bargaining unit members?
> 		- If yes, are those employees more or less senior than the employee previously doing that work?
> 		- If yes, will these be newly-hired employees?
> 		- If yes, will these be contracted employees? (If yes, please provide UVMSU with the contracts.)
> 	3) The position description of the Health Care Counselor Senior as it was when Jessica was in that position.
> 	4) In addition, we are requesting information about how salaries were determined for Healthcare Counselors in the Center of Health and Wellbeing: **Anne Desmond, Lindsey Foreman, Mary Heininger, and Olivia Sanders.** These employees all received notification of an equity increase on April 3, 2025.
> 		Please provide documentation of the following items for each individual:
> 		•	Years of UVM experience
> 		•	Years of non-UVM experience
> 		•	Education
> 		•	Hire date
> 		•	FTE
> 		•	Term
> 		•	Job Standard
> 		•	Minimum salary for the pay range
> 		•	Maximum salary for the pay range
> 		•	The percentile in which the individual falls in that current range
> 		•	Current hourly rate (actual)
> 		•	Current annual salary rate (actual)
> 		•	Current annual salary rate adjusted for shift differential
> 		•	Current annual salary rate adjusted for FTE and Term
> 		•	Salary justification (means and evidence for determining salary including complexity of role)
> 		- Including the original salary justifications prior to the April 3, 2025 equity adjustments.
> 		•	Any other materials relevant to determining salary placement
>  
> Sincerely,
> Jack Roberts
> UVMSU Lead Steward
> 


# Datasets and Sources
- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [x] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....

# Notes
General [[Union Data Request Notes]]


# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *<file_name>.xlsx*
Script File Name:    *20250414_HWBHealthcareCounselorSenior.R* 

Response Email Date:       *2025-04-14*
Response Email Subject:   *RE: Information Request:  CHWB Healthcare Counselor Senior*
