# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [x] Pull Data
- [x] Customize main.R script in union_data_requests R Project
- [x] Run R Script
- [x] Verify data accuracy/formatting
- [x] Format xlsx output
- [x] Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`
# Request

>**From:** Gallmeyer, Olive (they/them) [ogallmey@med.uvm.edu](mailto:ogallmey@med.uvm.edu)  
.  **Sent:** Monday, March 10, 2025 2:23 PM  
>**To:** HR Partners [HRPartners@uvm.edu](mailto:HRPartners@uvm.edu)  
>**Cc:** Jack Roberts [Jack.Roberts@uvm.edu](mailto:Jack.Roberts@uvm.edu)
>**Subject:** Information Request- OPSGs at LCOM
>
>With the knowledge and approval of UVM Staff United, I am writing to request information about salary data for all Office/Program Support Generalists at the Larner College of Medicine, including the below information:
>
> - Years of UVM experience
> - Years of non-UVM experience
> - Education
> - Hire date
> - FTE
> - Term
> - Salary at hire date
> - Current annual salary rate
> - Current annual salary rate adjusted for FTE and term
> - Current hourly rate
> - Salary justification (means and evidence for determining salary including complexity of role)
> - Minimum and maximum salary for the pay band
> - Any other materials relevant to determining salary placement
> 
> Thank you,
> 
> **Olive Gallmeyer** **(they/them)**  
> [ogallmey@med.uvm.edu](mailto:ogallmey@med.uvm.edu)
> Events & Programs Coordinator, Office of Inclusive Excellence
> Area Steward, UVM Staff United, LCOM (Cluster #6)

Received 2025-03-10
Response Due Date 2025-03-24

# Rafae Guidance/Feedback
- Years of UVM experience
	- **UV_ACTIVE_EMPLS**: “Yrs” column. I rename it to “Benefit Service Years” for clarity, since this field is derived from benefits service date
	- **UV_ACTIVE_EMPLS**: “Benefits Service Dt”. I include this just to show where the previous column comes from and to cover the “Hire Date” later on
- Years of non-UVM experience
	- We don’t explicitly give this, instead we provide the “Years of Relevant Experience” from the person’s PD.
	- Run the report in PeopleAdmin called “Position data - years of exp and salary justification” and use position number as the key between it and the UV_ACTIVE_EMPLS query
- Education
	- UV_HR_HERD_SURVEY2
	- Sort by newest to oldest
	- Delete future dated degrees
	- Vlookup degree info (both the “Item ID” field and the “Education Lvl – Personal Data” field as separate columns
- Hire date
	- Covered by benefits service date
- FTE
	- From UV_ACTIVE_EMPLS
- Term
	- From UV_ACTIVE_EMPLS
- Salary at hire date (We will provide their salary/wage as of the date they entered their current position number since we don’t properly track hire date.)
	- Run **UV_ICJ_POSN_ENTRY_WAGE_SAL**
		- If *Group* == *KRO* Then *Position Entry Hrly Rate*
		- Else If *Group* == *SM1* Then *Position Entry Annual Rt*
	- The reason we don’t use exempt/non-exempt status for this decision is because non-exempt employees used to be paid a salary
	- Also include the “Posn Dt” field. Add a note that this is the date they entered their current position number.
- Current annual salary rate
	- From UV_ACTIVE_EMPLS (only if exempt, otherwise blank)
- Current annual salary rate adjusted for FTE and term
	- We don’t do this for them. Add a note in the email reply, “This can be calculated by the union using the information in this report”
- Current hourly rate
	- From UV_ACTIVE_EMPLS (only if non-exempt, otherwise blank)
- Salary justification (means and evidence for determining salary including complexity of role)
	- Run the report in PeopleAdmin called “Position data - years of exp and salary justification” and use position number as the key between it and the UV_ACTIVE_EMPLS query
	- Also add the “Salary Comments” field from this report
- Minimum and maximum salary for the pay band
	- Since these requests usually only include a single job code, I just look it up in the job code data in PeopleSoft
- Any other materials relevant to determining salary placement
	- N/A

# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *DataRequest_OffceProgSupport_LCOM_20250317.xlsx*
Script File Name:    *20250312_OPSG_LCOM.R* 

Response Email Date:       *2025-03-18*
Response Email Subject:   *RE: Information Request- OPSGs at LCOM*
