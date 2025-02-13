Monika Hotaling 

# 10,000 ft overview
- Get data from ETS week of 2/17
- Specific definition of how is allowed on the account/application, as the 'Responsible Official' for the TCS upload... 
- Two files IRS in XML format
	- One for one row per person
	- One for summary information (1094c) placed in the manifest xml. 
- Immediate checks on IRS upload
- ~week for accept/reject officially
	- Errors typically come from discrepancies betwen SSN office for household information. 
## Population
1. Anybody that has received bcbs at at any point. includes employees, former employees, and sometiimes non-employees
2. Anybody that qualified during the 12 or 11 month look back period. 
	1. Discrepancy between people recieving letters and those that qualify. 
		1. Kiki's benefit team tracks these people in excel spreadsheet. TODO:

Benefits Workscenter -> ACA Reports & IRS Forms
	Employee transmittal data
		 the data set with the PS forms containing data
		Presents the data holding all form data
		Note the effective update date for the creation of the additional row
		The process status shows how the form was cretead/status
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
	Transmission Errors provides erros on individu
1095c% for the public 
