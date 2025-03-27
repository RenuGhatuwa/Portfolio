Payroll Data Descriptive Analytics for the City of Vancouver

Project Title: Payroll Data Descriptive Analytics Platform using AWS

Objective:  
The objective of this project is to design a cloud-based analytics platform that enables the City of Vancouver to perform descriptive analysis on payroll data. The platform provides insights into workforce structure, compensation distribution, and payroll classification through data profiling, summarization, and storage in a structured format.

Background:  
The City of Vancouver previously managed payroll documentation at its site location but this practice blocked potential data analysis and restricted its growth as well as operational flexibility. The city found itself unable to process data effectively or report results promptly because of the various constraints present. AWS provided the necessary tools to upgrade payroll data management through cloud services which solved these efficiency problems. Strategic planning for workforce development alongside informed decision-making becomes achievable because AWS advances the understanding of employee categories and payroll allocations and compensation records.

Dataset:  
The dataset contains structured payroll information, including employee roles, wage ranges, classification types, and organizational groupings. The data was anonymized and generalized for analysis and reporting.

Methodology:

1. Data Ingestion:  
Raw payroll files in CSV format were securely ingested into Amazon S3 using encrypted channels and predefined pipeline configurations to ensure data integrity and accessibility.
![drawio](https://github.com/user-attachments/assets/a95609c1-fa5b-4784-a93e-19e9ac9442de)

3. Data Profiling and Assessment:  
The datasets were evaluated using AWS Glue DataBrew, which identified field types, missing values, statistical abnormalities, and problems with data quality. The groundwork for precise transformation was laid by the profile reports the tool produced, which gave a summary of record counts, column distributions, and outlier detection.
![data profiling](https://github.com/user-attachments/assets/145195d8-572d-408b-aa72-d761f963a75e)


4. Data Cleaning and Standardization:  
Low-variance columns were removed. Fields were renamed, date formats normalized, and categorical values standardized (e.g., employee group names, job status).
<img width="252" alt="cleaning recipes" src="https://github.com/user-attachments/assets/482bb8e7-145e-4bb4-ae28-ce54df9fe5e6" />

5. Data Summarization:  
The cleaned data was summarized to show counts by classification, distribution across wage ranges, and department-level breakdowns. Outputs were structured for use in dashboards and reports.
<img width="468" alt="pipeline visual etl" src="https://github.com/user-attachments/assets/5c327328-1c86-4ae5-bc05-56792a3e913e" />

6. Data Storage and Cataloging:  
Cleaned and summarized data was stored in Amazon S3, organized by usage type and partitioned by time. AWS Glue crawlers were configured to catalog the datasets for downstream querying via Amazon Athena.
![cataloging](https://github.com/user-attachments/assets/1b0c8ebd-782d-4409-bb55-b5c523d91923)

7. Validation and Documentation:  
Outputs were validated by inspecting row counts, schema integrity, and classification distributions. Visual documentation of the workflow and lifecycle policies was maintained throughout the process.

Tools and Technologies:  
- Amazon S3  
- AWS Glue DataBrew  
- AWS Glue Data Catalog  
- Amazon Athena  
- Lifecycle policies for cost optimization

Deliverables:  
- A structured, cloud-based payroll data repository  
- Cleaned and summarized payroll datasets for reporting  
- Metadata catalog accessible for ad-hoc queries  
- Data profiling reports and transformation history  
- Visual documentation of the pipeline and storage logic

Timeline:  
Completed in approximately 2 weeks, including ingestion setup, transformation workflows, and validation.

Outcome:  
The City of Vancouver enhances its workforce financial data management abilities through a properly deployed AWS-based payroll data analytics platform. A cloud-based architecture provides the city with three essential benefits: scalable storage together with automatic data transformation and on-demand querying features. The cleaned systematic records help organizations gain full visibility into their worker demographics while showcasing departmental wage patterns along with payroll classification types. The delivery of financial planning and budgeting procedures improves through rapid decision support from analysts who generate reports on-demand using Amazon Athena alongside AWS Glue. Through its establishment the platform supports sustainable public resource management by providing data-based decisions and clear payroll transparency mechanisms.

