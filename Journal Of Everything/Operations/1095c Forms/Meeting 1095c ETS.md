Monika Hotaling 

# 10,000 ft overview
- Get data from ETS week of 2/17
- Specific definition of how is allowed on the account/application, as the 'Responsible Official' for the TCS upload... 
- Two files IRS in XML format
	- One for one row per person
	- One for summary information (1094c) placed in the manifest xml. 
- Immediate checks on IRS upload
- ~week for accept/reject officially
	- Errors typically come from discrepancies between SSN office for household information. 
## Population
1. Anybody that has received bcbs at at any point. includes employees, former employees, and sometimes non-employees
2. Anybody that qualified during the 12 or 11 month look back period. 
	1. Discrepancy between people receiving letters and those that qualify. 
		1. Kiki's benefit team tracks these people in excel spreadsheet. TODO:

Benefits Workscenter -> ACA Reports & IRS Forms
	Employee transmittal data
		 the data set with the PS forms containing data
		Presents the data holding all form data
		Note the effective update date for the creation of the additional row
		The process status shows how the form was created/status
		1 series data shows who was offered insurance and why.
		Employee Monthly amounts shows the lowest cost option
			COMMON PLACE FOR CORRECTIONS
		Currently used for updating records -- possible for mass upload but hasn't been tested in a long time
		Safe harbor i.e. 1 series codes dependent on benefits processing data. 
	Eligibility Report
		Requires manual load
		To be determined must have the non-assessment period checked. Drives the 2 series 2D designation. 
		Hours worked, and date fields are irrelevant
		Required for form creation. 
	ACA Employer Transmittal Data
		used for manifest summary data
	Transmission History provides info transmission data
	Transmission Errors provides errors on individual rows
1095c% for the public 

## Review of supplied dataset
UVM 1095c 
Dependents are not 00 or blank
Benenfit census date as the book of truth but doesn't contain the dpendent information
	Run Jan 31, Jul, Dec 31 for medical election data.
Compare offer letter cost to lowest cost option.
Check ACA FT Elig against letter sent list

Benefit program A01, B01, C01, etc - UVM elig A, B, C etc
