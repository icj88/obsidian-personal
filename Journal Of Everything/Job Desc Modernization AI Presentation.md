## Why?
What HR Projects or processes are suitable for AI/LLMs?
Proof of concept for AI/LLM use.
## What?
Translating existing Job Description content from percentage to outcome based content.
Highly suitable for AI:
- Large scope: thousands of pages of jds requiring conversion.
- Use of existing data: minimizes hallucination risks
- Tailored format and instructions: customizable output formats and other instructions
## How?
### What goes on under the hood...
#### Define the input content
   `Input: Traditional percentage-based job description with job summary and function percentages and responsibilities`
   
#### Define the output format
```
Transform input content job description into structured markdown following this schema and only this schema:

# [Position Title]

## Role Summary
[Core purpose and impact]

## Key Responsibilities
For each major responsibility area (indicated by percentage):
### [Area Name]
- Primary Outcomes:
  - [What this area achieves]
- Key Activities:
  - [Main tasks and processes]

## Success Indicators
- [Measurable outcomes from the responsibilities]
```

#### Provide translation instructions
```
Transformation Rules:
	1. Convert time percentages into priority weighting
	2. Consolidate all Low priority responsibility areas into single 'Additional Responsibilities'
	3. Group related tasks under their primary responsibility
	4. Extract concrete success indicators from task descriptions
```

#### Feed Job Description data from PeopleAdmin
##### Example input:
```html
content = "<div>The HR Analyst plays a crucial role in providing analytical, data, and HR systems reporting support across the Campus. Advise HR colleagues, coordinate and execute data initiatives, and collaborate with various institutional functions to ensure the alignment of HR data with business objectives. Collaborate with Information Technology to standardize reporting queries and ensure data accuracy. Provide analytical support for institutional and HR initiatives, including data gathering, manipulation, synthesis, and interpretation. Conduct internal measurements and metrics analyses, such as employee turnover trends and benchmarks, to monitor HR programs. Assist Classification &amp; Compensation group with special excel-based projects. Report to the HR Technology and Data Manager.</div>	<div><strong>Provide Analytical Support – 25% </strong>Provide analytical support for institutional and HR initiatives, including data gathering, manipulation, synthesis, and interpretation. Conduct internal measurements and metrics analyses, such as employee demographics, turnover trends, and benchmarks, to monitor HR programs. Deliver independent business analysis for HR functions, focusing on data management and reporting.</div>, <div><strong>Provide Reporting Support – 25% </strong>Design and develop queries for reporting and special projects, utilizing the HR systems and other reporting tools. Collaborate with the HRIT Lead Analyst and business owners to identify process and data improvement opportunities. Lead requirements gathering, development, maintenance, and communication of HR analytics and reports.</div>, <div><strong>Provide Systems Support – 15% </strong>Provide first-level support for inquiries related to HR systems. Follow established processes to audit HR data routinely.</div>, <div><strong>Ensure Data Governance and Integrity – 15% </strong>Maintain, formulate and implement processes for maintaining data quality, integrity, and consistency within departmental and HR systems. Lead data initiatives to define, standardize, cleanse, and map HR data, ensuring alignment with business processes.</div><div><br></div>, <div><strong>Stakeholder Interaction and Collaboration – 10%</strong>Interface with departments on Campus requiring HR data, delivering value-added service aligned with business objectives. Collaborate with Information Technology to standardize reporting queries and ensure data accuracy. Collaborate with the Office of Institutional Research and Assessment and ensure data alignment with business objectives.<br><br></div><div><br></div>, <div><strong>Training – 5%</strong>Create data and report-related user documentation and conduct training as needed.</div><div><br></div>, <div><strong>Perform additional assigned duties as needed – 5%<br></strong><br></div>"
```

##### Example output:
[[Job  Desc Modernization Formatted Example]]
```
=== Gemini Response ===

## Role Summary
The HR Analyst provides crucial analytical, data, and HR systems reporting support, ensuring HR data aligns with business objectives and contributing to the effectiveness of HR programs.

## Key Responsibilities

### Analytical Support
- Primary Outcomes:
  - Provide data-driven insights to support institutional and HR initiatives.
  - Monitor HR program effectiveness through internal measurements and metrics.
- Key Activities:
  - Gather, manipulate, synthesize, and interpret data for analysis.
  - Conduct internal measurements and metrics analyses, such as employee demographics, turnover trends, and benchmarks.
  - Deliver independent business analysis for HR functions, focusing on data management and reporting.

### Reporting Support
- Primary Outcomes:
  - Develop and maintain effective HR reports and analytics.
  - Identify and implement process and data improvements.
- Key Activities:
  - Design and develop queries for reporting and special projects, utilizing HR systems and other reporting tools.
  - Collaborate with the HRIT Lead Analyst and business owners to identify process and data improvement opportunities.
  - Lead requirements gathering, development, maintenance, and communication of HR analytics and reports.

### Data Governance and Integrity
- Primary Outcomes:
  - Maintain high data quality, integrity, and consistency within HR systems.
  - Ensure HR data is standardized, cleansed, and mapped for alignment with business processes.
- Key Activities:
  - Maintain, formulate, and implement processes for maintaining data quality, integrity, and consistency within departmental and HR systems.
  - Lead data initiatives to define, standardize, cleanse, and map HR data.

### Systems Support
- Primary Outcomes:
  - Provide timely and effective first-level support for HR system inquiries.
  - Ensure data accuracy through routine audits.
- Key Activities:
  - Provide first-level support for inquiries related to HR systems.
  - Follow established processes to audit HR data routinely.

### Additional Responsibilities
- Primary Outcomes:
  - Support HR data needs across the institution.
  - Ensure data alignment and accuracy through collaboration.
  - Provide necessary training and documentation.
- Key Activities:
  - Interface with departments on Campus requiring HR data, delivering value-added service aligned with business objectives.
  - Collaborate with Information Technology to standardize reporting queries and ensure data accuracy.
  - Collaborate with the Office of Institutional Research and Assessment and ensure data alignment with business objectives.
  - Create data and report-related user documentation and conduct training as needed.
  - Perform additional assigned duties as needed.

## Success Indicators
- Accurate and timely delivery of HR reports and analytics.
- Identification and implementation of data and process improvements.
- Maintenance of high data quality and integrity within HR systems.
- Effective first-level support for HR system inquiries.
- Positive feedback from stakeholders on data support and collaboration.
- Completion of data and report-related user documentation and training.
```


### How the user interacts...
#### Customizations
**Define input content,** i.e. what job attributes should be included in addition to the previous job description? FTE, CPD Family, SubFamily, Career Path, Career Level, etc.

**Define output content**, i.e. what is the output document structure including headings/sections and brief section descriptions.  

**Define translation instructions**, i.e. how should data be consolidated, what rules should be applied when deciding what to include or not include, how should the model handle missing information?
#### Common Information
Information that will be supplied to each translation...
- CPD definitions
- Example 'ideal' translation(s)
## What next?
**Define Output Content**: Create a job description template(s)
**Refine Instruction Set**:  Align instruction set with desired output content.
**Produce 'Ideal' translation:** Produce one or two ideal translations to better guide the LLM.
