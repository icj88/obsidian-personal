## Setup Dedicated DB Environment
- Consult with ETS - Maggie Caldwell, Susan Skalka
- Data sourced from Production PeopleSoft and Monthly BCBS datasets. 
	1. Example BCBS: ***A856_UVM_2023_PROD_120906928.xlsx***

***TODO***: Formalize the business logic that is being used to create the datasets. Filtering and rules used for fields in the final *UV_BN_ACA_1095C_Data* report from the dedicated db environment.

## Flag Records for Review


## Update Data in Dedicated DB Environment



## Steps for Annual ACA Processing
1.  Setup 1095C Database environment in PeopleSoft.
1. Populate database tables (ETS, Maggie Caldwell, Susan Skalka)
2. Run **UV_BN_ACA_1095C_Data** for the appropriate calendar year
3. Clean and fill missing data
	1. Create new dataset with primary subscriber only rows. These are indicated by rows whose DEP values are not *NA* or *'00'*
	2. 
