# Data Request Checklist
- [ ] Determine response Deadline (typically, 10 business days)
- [ ] Review request 
	- [ ] Are the requested fields available?
	- [ ] Are the requested fields shareable?
	- [ ] Does the requestor have authority for the request?
	- [ ] Is the request satisfied using the standard template?
- [ ] Provide initial follow-up to business partner or requestor (if received directly)
- [ ] Create Entry in Obsidian [[Union Data Request Index]]
- [ ] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
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

> Quoted Original Email from the original requestor (if not in the primary request section)

# Datasets and Sources
- [ ] UV_ACTIVE_EMPLS [General EE Info]
- [ ] UV_HR_HERD_SURVEY2 [Education]
- [ ] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [ ] UV_KEYREP_RPT_QRYAMNEW_PRIMPUB [Salary/Wage Band Min/Max]
- [ ] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....

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
- Salary at hire date (We will provide their salary/wage as of the date they entered their current position number since we don’t properly track hire date.)
	- Run **UV_RK_ANNUAL_RT_POSN_ENTRY**
	- If *Group* == *KRO* Then *Position Entry Hrly Rate*
	- Else If *Group* == *SM1* Then *Position Entry Annual Rt*
	- The reason we don’t use exempt/non-exempt status for this decision is because non-exempt employees used to be paid a salary
	- Also include the “Posn Dt” field. Add a note that this is the date they entered their current position number.

# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *<file_name>.xlsx*
Script File Name:    *<script_file_name>.R* 

Response Email Date:       *<YYYY-MM-DD\>*
Response Email Subject:   *RE: <Email Subject Line\>*
