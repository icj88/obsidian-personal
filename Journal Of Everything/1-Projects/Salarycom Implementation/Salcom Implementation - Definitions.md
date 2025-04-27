## Full-time / Part-time
Part-time = FTE < 1.0
Full-time  = FTE  == 1.0

## Company Job Code
### Salary.com Job Code Definition
*'Each unique job should have its own unique Job Code. For example - Job Accountant could have a job code of 0001A. There is one job, but it may have three incumbents or positions within that job.*

*Example: Persons 1, 2, and 3 are all Accountants and they do the exact same job and are market priced the same. They all share the job code of 0001A.*

*NOTE: Problems can occur if you have two different job codes for the same job. An example of this if Person 1 and 2 were both Accountants and performed the same job and had similar pay, but person 2 has a job code of 000B1.*

*When you price job code 0001A against the market you will also have to market price 000B1 when you could have done it once for one job code.*

*The reverse of this can also occur when you generalize job codes. You may have two employees with the same job code 000AA - Director, but they actually have different jobs. One is Director of Finance and the other is Director of Operations. Two different jobs should have two different job codes.*

### Internal Mapping
People Soft Job Code


## Salary Grade
### Salcom Definition
*Grade codes are used in CompAnalyst to align pay ranges to specific jobs in reporting and modeling. Grade codes are grouped under Structures. If Grades do not exist at the time of implementation, a placeholder Grade must be defined and linked to a Structure in order for reports and data to properly link.*
### Internal Assignment
Set to Career Stream - Career Level

## Salary Plan Code
*Salary Plan Codes are used in CompAnalyst to allow for the differentiation of salary ranges based on different pay markets or other groupings. If Salary Plans do not exist at the time of implementation, a placeholder Salary Plan must be defined and linked to a Structure in order for reports and data to properly link.*

*Example: A client has an Exempt Structure with Grades A,B,C. The values in Salary Range A may be different depending on whether an employee is based in New York City or Boston.*

*In that case, New York City and Boston would be defined as Salary Plans.*
### Internal Mapping
Currently Set as 'DEF' - 'Default Plan Code'

## Salary Structure
### Salcom Definition
*A Structure in CompAnalyst is a grouping of client pay grades. If Structures do not exist at the time of implementation, a placeholder Structure must be set up in order for reports and data to properly link.*
### Internal Mapping
FLSA Status - Union
