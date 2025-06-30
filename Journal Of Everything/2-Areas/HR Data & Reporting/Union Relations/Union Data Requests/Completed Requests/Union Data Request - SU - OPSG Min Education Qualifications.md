# Data Request Checklist
- [x] Determine response Deadline (typically, 10 business days)
	- [x] June 18, 2025
- [x] Review request 
	- [x] Are the requested fields available?
	- [x] Are the requested fields shareable?
	- [x] Does the requestor have authority for the request?
	- [x] Is the request satisfied using the standard template?
		- [x] No, minimum qualifications only with hourly rates
- [x] Provide initial follow-up to business partner or requestor (if received directly)
- [x] Create Entry in Obsidian [[Union Data Request Index]]
- [x] Determine data sources (PeopleSoft, PeopleAdmin, Payroll, or others)
- [x] **(NA)** Customize main.R script in union_data_requests R Project
- [x] Pull Data
- [x] **(NA)** Run R Script
- [x] Verify data accuracy/formatting
- [x] Format xlsx output
- [x] **(NA)** Email CompClass for final review/revision, cc Rafae, Caroline, Requestor
- [x] **(NA)** Save updated main.R as new file in `/union_data_requests/Requests/` with the name `YYYYMMDD_RequestDescription.R`

# Request

>Hi Amanda, 
>
>The attached dataset contains the minimum qualifications for all Active or Posted Office/Program Support Generalist Positions.
>
>Four positions contain language indicating a higher than associate’s degree minimum. They are highlighted in yellow in the workbook and contain unit/dept information and hourly rates. 
>
>Nothing about these positions struck me as particularly notable. The hourly rates were not outliers among OPSG positions, and they are distributed in differing units and departments. 
>
>Please let me know if there is anything that requires clarification.
>
>Ian
---
>
>From: Rafae Khan <Rafae.Khan@uvm.edu> 
>Sent: Thursday, June 5, 2025 10:58
>To: Amanda McIntire <Amanda.McIntire@uvm.edu>
>Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
>Subject: RE: Information Request- OPSG Minimum Educational Qualifications
>
>Sorry, missed your question. I honestly don’t know what the min quals should be for these positions. 
>
>According to the job standard on the class & comp site, it would be an associate’s degree.
>
>https://www.uvm.edu/d10-files/documents/2024-10/CareerPay-AdminSupportFamily.pdf
---
>From: Rafae Khan 
>Sent: Thursday, June 5, 2025 10:56 AM
>To: Amanda McIntire <Amanda.McIntire@uvm.edu>
>Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
>Subject: RE: Information Request- OPSG Minimum Educational Qualifications
>
>Thanks Amanda!
>
>Just to confirm, when they ask for “unfilled” positions, we typically would only provide that for posted jobs. There are many vacant positions that the units simply haven’t deactivated. Are you good with that?
>
----
>From: Amanda McIntire <Amanda.McIntire@uvm.edu> 
>Sent: Thursday, June 5, 2025 9:43 AM
>To: Rafae Khan <Rafae.Khan@uvm.edu>
>Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
>Subject: RE: Information Request- OPSG Minimum Educational Qualifications
>
>Thank you, Rafae and Ian!
>
>Understood on the “equivalent combination” language, which in my mind (oversimplified) means we can hire an applicant with a bachelor’s degree and less experience- or a person with a GED and lots of experience for an OPSG position. However, I don’t think any of the OPSG positions should list a degree requirement that is higher than an Associate’s. Is this your understanding? It is an interesting ask – I wish I knew what situation they are looking into. Perhaps Ian will discover it for us. 
>
>Thanks again, 
>Amanda
---
>From: Rafae Khan <Rafae.Khan@uvm.edu> 
>Sent: Thursday, June 5, 2025 9:24 AM
>To: Amanda McIntire <Amanda.McIntire@uvm.edu>
>Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
>Subject: RE: Information Request- OPSG Minimum Educational Qualifications
>
>Hi Amanda:
>
>We can pull the min quals for positions, but I would want to make it clear that none of our OPSG positions are ever posted with a true degree requirement. The minimum qualifications field specifically states “or equivalent combination of education and experience”. I may be picking nits, but I think it is an important distinction.
>
>Ian, will you be able to pull this? You can pull the PD information as normal and filter on the minimum qualifications field. Then I would compare it to a list of positions with an incumbent and the list of posted OPSG positions.
>
>-Rafae
---
>From: Amanda McIntire <Amanda.McIntire@uvm.edu> 
>Sent: Thursday, June 5, 2025 8:59 AM
>To: Rafae Khan <Rafae.Khan@uvm.edu>
>Cc: Caroline Cote (she/her) <Caroline.Cote@uvm.edu>; Ian Johnson <Ian.C.Johnson@uvm.edu>
>Subject: FW: Information Request- OPSG Minimum Educational Qualifications
>
>Good Morning Rafae and team, 
>Below, you will find an information request we received from UVMSU.
>Is this something you can assist with? 
>Please let me know what you think. It is due on June 18. 
>Thank you, 
>Amanda
>
>
>AMANDA MCINTIRE
>HR Partner
----
>From: Olive Gallmeyer (they/them) [LCOM] <ogallmey@med.uvm.edu> 
>Sent: Wednesday, June 4, 2025 1:34 PM
>To: HR Partners <HRPartners@uvm.edu>
>Subject: Information Request- OPSG Minimum Educational Qualifications
>
>Good afternoon,
>
>With the knowledge and support of UVM Staff United, I am writing to request information about the minimum qualifications required for Office/Program Support Generalist positions, including the below information:
>
>•	Number of positions in the Office/Program Support Generalist role (filled or unfilled) that list educational qualifications higher than an associate’s degree as minimum qualifications
>•	Unit and department of any OPSG positions that require educational qualifications higher than an associate’s degree
>•	Hourly salary rate of any positions (or, for unfilled positions, anticipated pay range) that require educational qualifications higher than an associate’s degree
>
>Thank you,
>
>OLIVE GALLMEYER (they/them)

## Original

>From: Olive Gallmeyer (they/them) [LCOM] <ogallmey@med.uvm.edu> 
>Sent: Wednesday, June 4, 2025 1:34 PM
>To: HR Partners <HRPartners@uvm.edu>
>Subject: Information Request- OPSG Minimum Educational Qualifications
>
>Good afternoon,
>
>With the knowledge and support of UVM Staff United, I am writing to request information about the minimum qualifications required for Office/Program Support Generalist positions, including the below information:
>
>•	Number of positions in the Office/Program Support Generalist role (filled or unfilled) that list educational qualifications higher than an associate’s degree as minimum qualifications
>•	Unit and department of any OPSG positions that require educational qualifications higher than an associate’s degree
>•	Hourly salary rate of any positions (or, for unfilled positions, anticipated pay range) that require educational qualifications higher than an associate’s degree
>
>Thank you,
>
>OLIVE GALLMEYER (they/them)

# Datasets and Sources
- [ ] UV_ACTIVE_EMPLS [General EE Info]
- [ ] UV_HR_HERD_SURVEY2 [Education]
- [ ] PA - Position data - years of exp and salary justification [Years of Relevant Experience and Salary Justification]
- [ ] UV_ICJ_JOBCODETBL_ALL [Salary/Wage Band Min/Max]
- [ ] UV_RK_ANNUAL_RT_POSN_ENTRY [Salary/Wage at Time of position entry]
- [ ] Others....
- [x] PD Position Search
# Notes
General [[Union Data Request Notes]]


# Response
Compiled via newly created union_data_requests R Project. 

Output File Name:  *OPSG_Min_Quals_20250605.xlsx*
Script File Name:    *None* 

Response Email Date:       *2025-06-05*
Response Email Subject:   *RE: Information Request- OPSG Minimum Educational Qualifications*
