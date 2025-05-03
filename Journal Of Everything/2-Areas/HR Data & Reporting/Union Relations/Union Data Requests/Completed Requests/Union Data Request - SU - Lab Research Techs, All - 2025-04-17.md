# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	- May 1st 
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
		- **No**, this required the original, rather than the most recent, Salary Justification and HR Comments.  
		- Request to include Dept and FSCM Rollup by Matthew
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
**From:** Matthew Casey [Matthew.Casey@uvm.edu](mailto:Matthew.Casey@uvm.edu)
**Sent:** Thursday, April 17, 2025 10:18 AM  
**To:** Rafae Khan [Rafae.Khan@uvm.edu](mailto:Rafae.Khan@uvm.edu); Ian Johnson [Ian.C.Johnson@uvm.edu](mailto:Ian.C.Johnson@uvm.edu)
**Cc:** Caroline Cote (she/her) [Caroline.Cote@uvm.edu](mailto:Caroline.Cote@uvm.edu)  
**Subject:** Fw: Information Request: Laboratory Research Technicians in Geo and other departments/colleges

Good morning,
Please see the information request below for all Lab Research Technicians across the university (should be approx. 120 records). 
Note the request for the original salary justification at time of hire, rather than the most recent position action. 
Let me know if you have any questions. Thanks!

Matthew Casey **(he/him/his)**  
_HR Partner_  
Human Resources  
University of Vermont  
Room 228 - Waterman| 85 S. Prospect St  
Burlington, VT 05405   
[matthew.casey@uvm.edu](mailto:matthew.casey@uvm.edu)

## Original
**From:** Andy Aquino (she/her) [Andrea.Aquino@uvm.edu]
**Sent:** Tuesday, April 15, 2025 3:40 PM  
**To:** HR Partners [HRPartners@uvm.edu]
**Cc:** Jack Roberts [Jack.Roberts@uvm.edu]
**Subject:** Information Request: Laboratory Research Technicians in Geo and other departments/colleges
Hello, 
With the knowledge and support of UVMSU, per Article 23.9c, we are requesting information about how salaries were determined for **Ken Johnston** and **Saul Blocher** (Laboratory Research Technicians in Geology & Geosciences). As these two are the only employees with that title in Geo, we also ask for salaries for other Laboratory Research Technicians across the University including other departments, Rubenstein, CALS, etc.

Please provide documentation of the following items for each individual:

- Years of UVM experience
- Years of non-UVM experience
- Education
- Hire date
- FTE
- Term
- Job Standard
- Minimum salary for the pay range
- Maximum salary for the pay range
- The percentile in which the individual falls in that current range
- Current hourly rate (actual)
- Current annual salary rate (actual)
- Current annual salary rate adjusted for shift differential
- Current annual salary rate adjusted for FTE and Term
- Proposed annual salary (actual) after equity review
- Percent increase (if proposed) between current annual salary rate (actual) and proposed annual salary (actual) after equity review
- Salary justification (means and evidence for determining salary including complexity of role)
- Any other materials relevant to determining salary placement

In addition, if raises were given to staff members in this group, I request the original salary justification for the employees be provided. I have observed that sometimes the original salary justification can get overridden to just mention a recent raise.

Thank you very much!  
Andy

**Andrea Aquino** (she/her)
administrative assistant
_Music Program, School of the Arts_
_University of Vermont_
_(802) 656-2295_
_Southwick 200 C_

# Datasets and Sources
- [x] UV_ACTIVE_EMPLS [General EE Info]
- [x] UV_HR_HERD_SURVEY2 [Education]
- [x] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [x] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [x] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [x] PA - Hiring Proposal Report for AAP [Original Salary Justification and Comments]
- [ ] Others....

# Notes
General [[Union Data Request Notes]]


# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *DataRequest_AllLabReserchTechs_20250430.xlsx*
Script File Name:    *20250430_LabRsrchTechs_All.R* 

Response Email Date:       *2025-05-02*
Response Email Subject:   *RE: Information Request: Laboratory Research Technicians in Geo and other departments/colleges*
