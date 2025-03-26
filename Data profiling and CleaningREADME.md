# Data Quality Control for Academic User Logs – UCW Project

## Project Title: Implementation of Data Quality Control Measures for Academic Logs at UCW


Objective:  
To establish a robust data quality control framework for managing academic user log data stored in Amazon S3. The focus is on ensuring accuracy, completeness, consistency, and long-term integrity through profiling, cleaning, validation, and lifecycle rules using AWS Glue DataBrew and S3.

Background:  
Academic systems at University Canada West collect detailed logs and records, which were previously unmanaged. This project implements a scalable solution to ingest, profile, clean, and monitor these logs in AWS, ensuring regulatory compliance and data readiness for analytics.

Dataset:  
- academics-user-log.txt: A structured log file with 50 rows and multiple attributes.  
- Additional datasets: Academic Report Forms, Student Lists, and Case Lists.

Methodology:

1. Current State Assessment  
- Analyzed user logs and academic data in AWS S3.  
- Identified data issues: inconsistent column structures and lack of validation checks.

2. Data Profiling (using AWS Glue DataBrew)  
- Identified column types, missing values, and duplicate rows.  
- Profiled datasets:
  - aca-reportform-list-ds-ren
  - Aca-Case-list-ds-ren
  - Aca-student-list-ds-ren
<img width="1440" alt="Data profiling 1" src="https://github.com/user-attachments/assets/35fa6bc5-3c26-4f8f-a68d-f6b43325a54c" />
<img width="1440" alt="Data Profiling 2" src="https://github.com/user-attachments/assets/c14a2718-b7a3-4466-95ad-607c693d331f" />

<img width="1440" alt="data profilin 3" src="https://github.com/user-attachments/assets/91b1cbc4-ae33-41b4-9d47-d54fe48b5895" />

3. Data Cleansing  
- Created DataBrew recipes and ran successful jobs to clean each dataset.  
- Standardized column formats and removed invalid rows.  

<img width="1440" alt="SS Data Cleaning" src="https://github.com/user-attachments/assets/2feeb6f5-dc52-4b45-bd88-c67ed6bac917" />


4. Validation Rules  
- Ensured data types matched schema expectations.  
- Verified no missing or duplicate values remained post-cleaning.

5. Monitoring and Reporting  
- Used DataBrew's built-in reports for profiling summaries.  
- Scheduled profiling jobs to run on demand.

6. Lifecycle Rules  
- Configured lifecycle policies in S3 for automatic archiving of student, case, and reportform data.  
- Transition rules include Glacier Instant and Standard-IA.
<img width="1440" alt="SS Lifecycle Rule" src="https://github.com/user-attachments/assets/1554be7a-bafd-43a4-a836-8e014cfa3b1d" />


Tools and Technologies:
- AWS S3
- AWS Glue DataBrew
- PowerShell
- draw.io
- Amazon S3 Lifecycle Management

Architecture Overview:  
The system integrates EC2 (for ingestion), S3 (for storage), and Glue DataBrew (for profiling and cleaning).



PowerShell Upload Command Used:
Write-S3Object -Bucket academics-raw-ren -File "C:\Users\Administrator\Documents\academics-user-log.txt" -Key "/academic misconduct/academics-user-log/Ingestion/year=2025/quarter=1/month=1/day=25/server=ASVS-ren/academics-user-log.txt"

<img width="1440" alt="Powershell" src="https://github.com/user-attachments/assets/fb6fd964-d779-4cad-a18f-273f23de670e" />

Deliverables:
- DataBrew profile reports and cleaning job outputs  
- Cleaned and validated log datasets  
- Lifecycle-enabled data lake structure

Timeline:
- Completed in under 2 weeks: profiling, cleaning, and lifecycle setup

Outcome:  
This project ensures continuous data quality and archival integrity of academic logs at UCW, supporting compliance and analytics.
