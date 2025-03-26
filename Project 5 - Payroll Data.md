Payroll Data Descriptive Analytics for the City of Vancouver

Project Title: Payroll Data Descriptive Analytics Platform using AWS

Objective:  
The objective of this project is to design a cloud-based analytics platform that enables the City of Vancouver to perform descriptive analysis on payroll data. The platform provides insights into workforce structure, compensation distribution, and payroll classification through data profiling, summarization, and storage in a structured format.

Background:  
The City of Vancouver's payroll records were previously stored on-premise, limiting visibility, scalability, and reporting capabilities. This project modernizes the system using AWS cloud services to enable descriptive analytics, allowing the city to understand historical payroll trends, employee classifications, and compensation structures.

Dataset:  
The dataset contains structured payroll information, including employee roles, wage ranges, classification types, and organizational groupings. The data was anonymized and generalized for analysis and reporting.

Methodology:

1. Data Ingestion:  
Raw payroll files in CSV format were uploaded to Amazon S3 using secure ingestion pipelines.

![drawio](https://github.com/user-attachments/assets/a95609c1-fa5b-4784-a93e-19e9ac9442de)

3. Data Profiling and Assessment:  
AWS Glue DataBrew was used to profile datasets and identify patterns such as missing values, field types, and outliers. Summary metrics included row counts, column distributions, and data type consistency.
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
The platform enables the City of Vancouver to perform descriptive analytics on payroll data, supporting better workforce planning, financial reporting
