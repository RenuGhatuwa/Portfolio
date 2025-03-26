Data Wrangling and Summarization for Academic Logs – UCW Project

Project Title: Academic Data Summarization and Transformation with AWS Glue

Objective:  
The objective of this project is to automate the transformation and summarization of academic-related data using AWS Glue Studio. The goal is to process raw input from cloud storage into organized, analysis-ready datasets that support reporting and operational insights.

Background:  
University Canada West (UCW) maintains various logs and case-related records in Amazon S3. These records were historically stored in raw form, limiting their utility for data-driven decisions. This project addresses that challenge by building an ETL pipeline that extracts, transforms, and loads data into summarized outputs using AWS Glue Studio.

Dataset:  
The project works with multiple datasets representing academic records and log files stored in S3. These datasets contain structured information used to monitor, track, and summarize institutional activities. For privacy and abstraction, specific fields are generalized.

Methodology:

1. Data Collection:  
Raw data is stored in Amazon S3, structured using logical folders by year, month, and day. Data sources are registered in the AWS Glue Data Catalog to enable secure and scalable access.

2. Data Assessment:  
Initial assessments ensured the data sources were complete, consistent, and well-formatted. Key considerations included schema validation, record count checks, and folder structure review.

3. Data Cleaning:  
Data was cleaned to remove duplication, resolve formatting inconsistencies, and align timestamp formats required for summarization and analysis.

4. Data Transformation:  
The ETL pipeline was designed using AWS Glue Studio's visual interface. Key transformations included:
- Schema normalization
- Record filtering
- Summarization timestamp insertion
- Format conversions
- Target preparation for loading outputs
 <img width="1440" alt="Week 4 Drawio (1)" src="https://github.com/user-attachments/assets/26d2de35-404f-4674-94a1-1dd85c14af7c" />

<img width="1440" alt="Student List summarization" src="https://github.com/user-attachments/assets/04fee211-99d3-4d9c-bacc-c9f134ef1716" />


5. Data Consolidation:  
The Glue job generated structured outputs for multiple stakeholder views. Output datasets were logically partitioned for system-level and user-level access, stored separately in S3 with metadata-enriched folders.

6. Documentation and Validation:  
Each step of the pipeline was verified with log output and S3 inspection. The design was documented using visual representations of the Glue workflow and screenshots of the job execution environment.

Tools and Technologies:  
- AWS Glue Studio  
- AWS Glue Data Catalog  
- Amazon S3  
- Visual ETL Interface

Deliverables:  
- Fully operational ETL pipeline in AWS Glue  
- Partitioned and cleaned summary datasets  
- Visual workflow documentation and confirmation logs  
- Folder-based S3 structure aligned to reporting needs

Timeline:  
Completed within 3 days, including design, testing, and deployment phases.

Outcome:  
The project delivers a scalable, low-maintenance solution for transforming raw academic records into structured summaries. It enhances operational visibility, reduces manual processing, and sets the foundation for ongoing automation and analytics.
