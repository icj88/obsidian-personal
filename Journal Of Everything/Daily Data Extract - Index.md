The Daily Data Extract will automate and centralize a data extraction from the PeopleSoft system  to the shared network drive. These datasets aggregated by entity



[[Daily Data Extract Fields]]
[[Daily Data Extract - Requirements - Use Cases]]
[[Daily Data Dump - Requirements - User Stories]]

# General Thoughts

- *Data Sources*: We primarily use the PeopleSoft HCM database.
- *Stakeholders*:  
	- Human Resources employee end-users, 
	- HR Business and Data Analysts,
	- IT Database Administrators and SQL Report Writers. 
- *Current Processes*: 
	- Access queries built by IT team to pull data. 
		- Downloads as XLSX. 
		- Does not include report metadata (i.e. the query used to pull the data). 
	- Analyst builds query using a GUI 
		- Can be shared, however not shared or viewable by default. 
	- Secondary reporting system is used for complex queries. 
		- Sources, sql not viewable
		- Potentially long runtimes
- *Pain Points*:
	- Non standardized column names
	- Lack of documentation
	- Redundant and/or hard to differentiate queries
	- Very manual extract process
	- xlsx format not easy for handling multiple files. 
	- Blackbox reporting also has no documentation 
	- Use of outdated query results by end HR users creating contradictory information