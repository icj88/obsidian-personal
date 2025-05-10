# How to Update Salary.com CompAnalyst Datasets
1. Get the Upload Templates:
	1. *CompAnalyst Data Template_Company Data.xlsx*
	2.  *Employee Upload.xlsx*
2.  Download Source Datasets:
	1. UV_ACTIVE_EMPLS
	2. Job Code Architecture (rarely updated, may use currently existing file)
3. Save datasets to `~/Documents/datasets/UV_ACTIVE_EMPLS` and `~/Documents/datasets/JobCode_Architecture`
4. Open Salcom R Project located at `~/Documents/projects/salcom/salcom.Rproj`
5. Run main.R script
6. Copy/paste data from output datasets found in `./output` directory to employee upload template
7. Check for job codes in Employee dataset that are not included in the 'company job' upload dataset (found on *CompAnalyst Data Template_Company Data.xlsx*)
8. Upload to [companalyst.salary.com](companalyst.salary.com)
	1. Header/Name icon (top right) -> Tools & Settings -> File Upload
	2. Upload datasets individually