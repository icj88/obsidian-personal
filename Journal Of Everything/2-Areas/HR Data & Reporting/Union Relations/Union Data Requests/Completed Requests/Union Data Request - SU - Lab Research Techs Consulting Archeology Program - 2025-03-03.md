# Data Request Checklist
- [ ] Determine response Deadline (typically, 10 business days)
- [ ] Review request 
	- [ ] Are the requested fields available?
	- [ ] Are the requested fields shareable?
	- [ ] Does the requestor have authority for the request?
	- [ ] Is the request satisfied using the standard template?
- [ ] Provide initial follow-up to business partner or requestor (if received directly)
- [ ] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [ ] Customize main.R script in union_data_requests R Project
- [ ] Pull Data
- [ ] Run R Script
- [ ] Verify data accuracy/formatting
- [ ] Format xlsx output
- [ ] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [ ] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`
# Request

> **From:** Matthew Casey <[Matthew.Casey@uvm.edu](mailto:Matthew.Casey@uvm.edu)>  
> **Sent:** Tuesday, March 4, 2025 8:54 AM  
> **To:** Rafae Khan <[Rafae.Khan@uvm.edu](mailto:Rafae.Khan@uvm.edu)>  
> **Cc:** Caroline Cote (she/her) <[Caroline.Cote@uvm.edu](mailto:Caroline.Cote@uvm.edu)>  
> **Subject:** Fw: Information Request: Lab/research Technicians in Consulting Archeology Program
> 
> Good morning!
> 
> See below information request. Let me know if you have any questions.
> 
> Best,
> 
> Matthew
> 
> Matthew Casey **(he/him/his)**  
> _HR Partner_

## Original

> **From:** Dana Health Sciences Library Circulation Dept <[Dana.Circulation@uvm.edu](mailto:Dana.Circulation@uvm.edu)>  
> **Sent:** Monday, March 3, 2025 3:50 PM  
> **To:** HR Partners <[HRPartners@uvm.edu](mailto:HRPartners@uvm.edu)>  
> **Cc:** Andy Aquino (she/her) <[Andrea.Aquino@uvm.edu](mailto:Andrea.Aquino@uvm.edu)>  
> **Subject:** Information Request: Lab/research Technicians in Consulting Archeology Program
> 
> Hello,
>  
> With the knowledge and support of UVMSU, we are requesting information about how salaries were determined for Lab/research Technicians in Consulting Archeology Program: Meghan Eaton, Fiona Haverland, Kathleen Kenny, Kevin Lambert, Geoffrey Mandel, and Elizabeth Pool.
>  
> Please provide documentation of the following items for each individual:
>   -	Years of UVM experience
>   -	Years of non-UVM experience
>   -	Education
>   -	Hire date
>   -	FTE
>   -	Term
>   -	Job Standard
>   -	Minimum salary for the pay range
>   -	Maximum salary for the pay range
>   -	The percentile in which the individual falls in that current range
>   -	Current hourly rate (actual)
>   -	Current annual salary rate (actual)
>   -	Current annual salary rate adjusted for shift differential
>   -	Current annual salary rate adjusted for FTE and Term
>   -	Proposed annual salary (actual) after equity review
>   -	Percent increase (if proposed) between current annual salary rate (actual) and proposed annual salary (actual) after equity review
>   -	Salary justification (means and evidence for determining salary including complexity of role)
>   -	Any other materials relevant to determining salary placement
>  
> In addition, one member reported that there were raises given to employees in the department. Our union has not been able to verify this information yet; including verifying if raises were given to bargaining unit members. Could you verify this? We always support departments raising employee salaries, but, we should be receiving notices that changes have occurred so we can enforce equity. If it is the case that bargaining unit members salaries were adjusted, please send us the information of salary comparisons before and after the raises. 
>  
> In addition, if raises were given to staff members in this group, I request the original salary justification for the employees be provided. I have observed that sometimes the original salary justification can get overridden to just mention a recent raise.
>  
> Sincerely,
> Jack Roberts
> UVMSU Lead Steward 

# Datasets and Sources
- [x] UV_ACTIVE_EMPLS
- [x] UV_HR_HERD_SURVEY2
- [x] PA - Position data - years of exp and salary justification
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB
# Rafae Feedback/Guidance
- Years of UVM experience
	- **UV_ACTIVE_EMPLS**: “Yrs” column. I rename it to “Benefit Service Years” for clarity, since this field is derived from benefits service date
	- **UV_ACTIVE_EMPLS**: “Benefits Service Dt”. I include this just to show where the previous column comes from and to cover the “Hire Date” later on
- Years of non-UVM experience
	- We don’t explicitly give this, instead we provide the “Years of Relevant Experience” from the person’s PD.
	- Run the report in PeopleAdmin - **“Position data - years of exp and salary justification”** and use position number as the key between it and the UV_ACTIVE_EMPLS query
- Education
	- **UV_HR_HERD_SURVEY2**
	- Sort by newest to oldest
	- Delete future dated degrees
	- Vlookup degree info (both the “Item ID” field and the “Education Lvl – Personal Data” field as separate columns
- Hire date
	- Covered by benefits service date
- FTE
	- From **UV_ACTIVE_EMPLS**
- Term
	- From **UV_ACTIVE_EMPLS**
- Job Standard
	- Include job code and job code description from **UV_ACTIVE_EMPLS**
- Minimum salary for the pay range
	- Since these requests usually only include a single job code, I just look it up in the job code data in PeopleSoft
	- Alternatively,  **UV_KEYREP_RPT_QRYAMNEW_PRIMPUB**
- Maximum salary for the pay range
	- Since these requests usually only include a single job code, I just look it up in the job code data in PeopleSoft
	- Alternatively,  **UV_KEYREP_RPT_QRYAMNEW_PRIMPUB**
- The percentile in which the individual falls in that current range
	- We don’t do this for them. Add a note in the email reply to Matthew, “This can be calculated by the union using the information in this report”
- Current hourly rate (actual)
	- From **UV_ACTIVE_EMPLS** (only if non-exempt, otherwise blank)
- Current annual salary rate (actual)
	- From **UV_ACTIVE_EMPLS** (only if exempt, otherwise blank)
- Current annual salary rate adjusted for shift differential
	- We don’t provide the rate, but we can provide the “Shift” column from **UV_ACTIVE_EMPLS**
- Current annual salary rate adjusted for FTE and Term
	- We don’t do this for them. Add a note in the email reply to Matthew, “This can be calculated by the union using the information in this report”
- Proposed annual salary (actual) after equity review
	- Add a note in the email reply to Matthew, “N/A, this is not an equity review”
- Percent increase (if proposed) between current annual salary rate (actual) and proposed annual salary (actual) after equity review
	- Add a note in the email reply to Matthew, “N/A, this is not an equity review”
- Salary justification (means and evidence for determining salary including complexity of role)
	- Run the report in PeopleAdmin called “**Position data - years of exp and salary justification**” and use position number as the key between it and the **UV_ACTIVE_EMPLS** query
- Also add the “Salary Comments” field from this report
	- Report in PeopleAdmin called “**Position data - years of exp and salary justification**”
- Any other materials relevant to determining salary placement
	- N/A

- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [x] UV_ICJ_POSN_ENTRY_WAGE_SAL [Salary/Wage at Time of position entry]
- [ ] Others....
# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *DataRequest_LabResarchTechs_ConsultingArcheology_20250314.xlsx*
Script File Name:    *20250303_LabRsrchTechs_ArcheoConsult.R* 

Response Email Date:     *2025-03-14*
Response Email Subject: *RE: Information Request: Lab/research Technicians in Consulting Archeology Program*