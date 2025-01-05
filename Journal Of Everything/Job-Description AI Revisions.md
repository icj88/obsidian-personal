## Goal
Revise/update staff job-descriptions (JDs) into a standardized modern format.

## Background
Current JDs (as opposed to broader position descriptions) utilize a percentage-time based format. 

Modern JDs, as described in [A New Approach to Writing Job Descriptions](https://archive.ph/wo6NL#selection-1117.5-1117.51)(Nieto-Rodriguez, 2023), focus on outcomes rather than rigid time or percent approaches. This provides greater flexibility as processes and technologies change within the organization. 

## Scope
The University of Vermont maintains JDs for each active staff employee. As of January 6, 2025 there are
- **2505** staff JDs,
- **450** words per JD,
- **1.1mil** words or 3,746 pages of descriptions.

Non Union Staff hold a smaller, but still significant portion:
- **646** unique JDs,
- **550** words per JD,
- **353k** words or 1,178 pages of descriptions.

Assuming an average review and revision time of 30min per job, the baseline estimate for manual revisions is **325 hours** for Non-Union Staff, and **1200 hours** for all Staff. 

## Leveraging LLM Assistance for Revisions
Large Language Models (LLMs), such as *OpenAI's ChatGPT o1*, *Google's Gemini 1.5*, or *Anthropic's Sonnet 3.5*, are particularly well suited reduce the needed number of work hours for this project. 

Scripted use of an LLM tool would provide translation from the traditional JD format to the new format using information contained in the current JD, and newly assigned Career Path Development career level and path attributes. Jobs lacking needed information will be flagged for closer review. 

Utilization of a broad set of job information via the LLM allows for high quality production of job descriptions using less work-hours. 

## Next Steps
### Estimate Token Costs
Estimate the number of input and output tokens needed to process job description revision. Token cost varies by model and generally range from $1-$10 per million tokens (depending on model quality and speed). Each job description revision task requires approximately 4k tokens. Total token costs for non-union staff will be on the order of $10-$100.

### Develop Python Testing and Processing Framework 
40 hours of Python script development time will be needed to build the framework for testing and processing the job descriptions. This framework can be applied to future LLM model batch utilization.





