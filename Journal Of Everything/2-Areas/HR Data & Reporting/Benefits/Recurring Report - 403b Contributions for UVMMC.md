# Schedule
* On demand, typically ~ Quarterly

# Source Reports
| **REPORT NAME**             | **REPORT  DETAILS**                                       |
| --------------------------- | --------------------------------------------------------- |
| Request spreadsheet         | Supplied by UVMMC                                         |
| UV_RK_UVMMC_403BCONT_YTD    | All months contributions in Year. <br>Use calendar year   |
| UV_HR_NID_PSID_DUMP         | Social Sec and EmplID                                     |
| UV_UVMMC_403BCONT_PP        | Monthly contribution, use most recent pay period end date |
| UV_BN_UVMMG_JOB7000_CONSENT | Response for consent to share                             |
# Process
1. Join UVM EmpliD to Request sheet by Social Security
2. Join The Consent response column (1 = Y, 2 = N)
	1. Filter UV_BN_UVMMG_JOB7000_CONSENT to remove 1095-C, 
	2. Treat '0' response as 'N', missing response
3. UV_UVMMC_403BCONT_U
	1. Use Calendar year
	2. Pivot, aggregate, sum 'Sum Ded MTD' for year to date sum
	3. rename  YTD 403b contribution
	4. Join sum to request sheet
4. Add 'Has Contributed in Year' column
	1. Y if has contributed, N if not
5. Pivot sum Monthly contribution, join by emplid, name sum column MM/DD/YYYY contribution
6. Join to request sheet
7. Delete numbers for non consented.
8. Investigate one-offs
9. 