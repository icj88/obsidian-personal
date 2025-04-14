# Data Sources
- [ ] [[Benefit Census Report]] (5th of every Month)
- [ ] UV_ICJ_NETIDS_ALL
- [ ] UV_ICJ_ACTIVE_EMPLS_WITH_ADDR
- [ ] UV_ICJ_ALL_PHONES
- [ ] UV_EMPL_ADDRESSES

The population is determined by filtering the Medical Benefit Census report to those individuals who are in the ‘current’ report as Enrolled, but not in the previous report as Enrolled. This can be updated as frequently as needed. (quarterly, monthly, weekly, etc)

The draft report Covers the Feb. 5, 2025 to March 5, 2025 date range.

The report relies on 5 PeopleSoft reports/queries:

- UV_ACTIVE_EMPLS (for preferred name and job specific information)
- UV_ICJ_NETIDS_ALL (for email addresses derived from netid)
- UV_ICJ_PREFERRED_PHONES (for the preferred contact phone number)
- UV_EMPL_ADDRESSES (for the address information, MAIL address type is prioritized, followed by HOME address type)
- UVM Reports -> Benefits Reports -> Benefits Census Report (to determine ‘new’ enrollees)

The compilation of the final report is largely hands off once the reports are downloaded. The UV_% reports could certainly be built as a single query, but I’d rather not deal with the query builder GUI when these queries already exist.

Some outstanding questions:

- How should missing data be handled? for example, some employees do not have a phone number entered into PS.
- Are there are any concerns about handling this semi-sensitive personal contact information?

Upload to:
  [Medical Benefit Census Reports-Care Management](https://uvmoffice-my.sharepoint.com/:f:/r/personal/97lpalas_uvm_edu/Documents/Benefits/Care%20Management/Medical%20Benefit%20Census%20Reports-Care%20Management?csf=1&web=1&e=iNCgRZ)