# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	- Orig Request May 1, **Due by May 14**
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

**From:** Amanda Desmond [Amanda.Desmond@uvm.edu](mailto:Amanda.Desmond@uvm.edu)  
**Sent:** Monday, May 5, 2025 13:28  
**To:** Rafae Khan [Rafae.Khan@uvm.edu](mailto:Rafae.Khan@uvm.edu); Ian Johnson [Ian.C.Johnson@uvm.edu](mailto:Ian.C.Johnson@uvm.edu)  
**Cc:** Caroline Cote (she/her) [Caroline.Cote@uvm.edu](mailto:Caroline.Cote@uvm.edu)  
**Subject:** FW: Information Request

Good afternoon,

Please see the information request below from UVMSU. Elizabeth followed up with 4 employees they would like this info for, but can you please verify that they’re the only employees with the Administrative Professional job title in those areas?

Thank you!

Amanda

-----

**From:** Elizabeth Dunford (she/her) [Elizabeth.Dunford@uvm.edu](mailto:Elizabeth.Dunford@uvm.edu)  
**Sent:** Thursday, May 1, 2025 9:52 AM  
**To:** HR Partners [HRPartners@uvm.edu](mailto:HRPartners@uvm.edu)  
**Cc:** Jack Roberts [Jack.Roberts@uvm.edu](mailto:Jack.Roberts@uvm.edu); Diana Naser [Diana.Naser@uvm.edu](mailto:Diana.Naser@uvm.edu)  
**Subject:** RE: Information Request

To clarify those employes are:

***Crispina Pincus***
***Ryan Gates***
***Blair Love***
***Judith Buxton***

Thank you!
Best,
Elizabeth

**elizabeth dunford** **(she/her)**  
_Operations Support Generalist_  

----

**From:** Elizabeth Dunford (she/her)  
**Sent:** Thursday, May 1, 2025 8:16 AM  
**To:** HR Partners [HRPartners@uvm.edu](mailto:HRPartners@uvm.edu)  
**Cc:** Jack Roberts [Jack.Roberts@uvm.edu](mailto:Jack.Roberts@uvm.edu); Diana Naser [Diana.Naser@uvm.edu](mailto:Diana.Naser@uvm.edu)  
**Subject:** Information Request

Hello,

With the knowledge and approval of UVMSU, I am writing to request information about how salaries were determined for the following individuals in their current positions, including:

- Years of UVM experience
- Years of non-UVM experience
- Education
- Hire date
- FTE
- Term
- Job Classification
- Minimum salary for the pay range
- Maximum salary for the pay range
- The percentile in which the individual falls in that current range
- Current Hourly Rate (actual)
- Current annual salary rate (actual)
- Current annual salary rate adjusted for shift differential
- Current annual salary rate adjusted for FTE and Term
- Salary justification (means and evidence for determining salary including complexity of role)
- Level of complexity (numeric value)
- Any other materials relevant to determining salary placement

For the following individuals:

All employees in UVMSU Cluster #8: Offices under The President/Provost/VP for Enrollment Management/VP of Faculty Affairs with the job title “Administrative Professional.”

Thank you,
Elizabeth Dunford

**elizabeth dunford** **(she/her)**  
_Operations Support Generalist_

# Datasets and Sources
- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [x] UV_ICJ_JOBCODETBL_ALL [Updated Salary/Wage Band Min/Max]
- [x] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....

# Notes
General [[Union Data Request Notes]]
Need clarification on the specific units that make up UVMSU Cluster #8. 
What the heck are the clusters? How are they defined?

Modified the script to pull min/max directly from Jobcode Table dump.
Compiled via union_data_requests R Project. 
# Response


Output File Name:  *DataRequest_AdminProfessionals_FinanceAdminPresFacAffairsEnrollMgmt.xlsx*
Script File Name:    *20250430_AdminProfessionals_Cluster8.R* 

Response Email Date:       *2025-05-15*
Response Email Subject:   *RE: Information Request>*
