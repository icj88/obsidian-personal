[[1095c Dataset Review Doc]]

## Project File Locations
C:\Users\ijohnson\OneDrive - University of Vermont\Documents\projects\aca_irs_filings
S:\hrs\BENEFITS\Medical\Affordable Care Act\IRS Filing

## Changes from previous years

## Pain Points
Part time faculty credit hour tracking, ACA offers
Custom business rules that differ from pre-built reporting: Terminations(!)
Manual loading of data into lookback period
Lack of logic in many process steps

Specific test environment used. 

Anybody enrolled for minimum 1 calendar day - TODO: Check if there is a minimum period for eligibility for 1095c
Also anybody waived and worked for one full time month 


## Data source
BCBS database dump
ETS compares to Peoplesoft. HR reviews discrepencies
Eligibility information - stability period, full time/ part time / admin period.

17th Feb. first draft data
March  final deadline

# Steps
Check ACA related logins at IRS.
Apply for [TCC](https://www.irs.gov/tax-professionals/affordable-care-act-aca-services) (Typically Caitlyn.)
Compile HR ACA Offer Letters in dedicated xlsx file.
Request previous year's data from BCBS, an on 2/12. 
Create 'Test' Data
'Scrub' BCBS vs UVM PeopleSoft data
'Scrub' ACA Hours Reports Data
	Copy and pasted data into xlsx, wtf
	XLSX macro to insert data into peoplesoft (ughhhh)
