Cloud-Based Payroll Analytics and Security Platform

Project Title: Design and Implementation of a Secure Cloud-Based Payroll Data Analytics Platform

Objective:  
To design and implement a secure and scalable cloud-based data analytics solution for the City of Vancouver's payroll information using AWS services. The platform focuses on storing, analyzing, and protecting sensitive payroll data while ensuring governance, availability, and system observability.

Background:  
The City of Vancouver’s growing demand for efficient payroll data analysis and integrity led to the development of a cloud-native analytics platform. The goal was to extract insights into workforce compensation patterns using Amazon Athena while ensuring security and governance through AWS Glue, CloudTrail, and KMS. The project also prioritized backup and recovery using S3 versioning and replication, and real-time monitoring through CloudWatch.

Dataset:  
The dataset contained payroll-related records such as job classifications, hourly pay rates, employment years, and workforce distribution across categories. Although specific details remain confidential, data analysis was performed on anonymized records stored in Amazon S3.

Methodology:

1. Architecture Design:  
   - Outlined high-level architecture leveraging AWS S3, Athena, Glue Studio, KMS, CloudTrail, and CloudWatch.  
   - Defined the interaction between data storage, analysis, encryption, monitoring, and logging.
    <img width="468" alt="dap architecture" src="https://github.com/user-attachments/assets/1b86a115-62ae-4076-b9e7-89fed6be2ed9" />

    

2. Data Analysis:  
   - Queried salary trends, pay ranges, and workforce size across job classifications using Amazon Athena.  
   - Insights derived included classification-level salary gaps, year-over-year salary changes, and distribution of employee roles.
![query](https://github.com/user-attachments/assets/74fff325-4d39-4da1-85d3-2b843c2d33b5)

3. Data Security Measures:  
   - Created a customer-managed KMS key for encryption.
    ![kms](https://github.com/user-attachments/assets/ac6e43a6-4b4e-4d99-b444-e596a474c344)

   - Enabled S3 default encryption, versioning, and replication to backup buckets.
      ![bucket versioning](https://github.com/user-attachments/assets/f562d6aa-d396-416e-8ca8-f606a1e7f0a7)
![replication rule](https://github.com/user-attachments/assets/45227cd8-f6ed-4387-8a42-c2cf49fc71c5)
![encryption](https://github.com/user-attachments/assets/7f789b9a-8584-405c-a83d-4fb85979a349)

   - Restricted decryption permissions to specific IAM roles.
    

4. Data Governance with AWS Glue Studio:  
   - Created ETL jobs with embedded quality rules (e.g., salary range validation, primary key checks).
   <img width="468" alt="quality check" src="https://github.com/user-attachments/assets/670ebe4d-28c1-47b7-b309-bb2b46b0ea02" />

   - Used conditional routing to separate valid and failed data for traceability.

5. Monitoring and Logging:  
   - Configured CloudWatch dashboards and alarms for tracking bucket usage and anomalies.
   ![dashboard](https://github.com/user-attachments/assets/352085e6-819a-4f93-9b3c-8504e0cab49c)

   - Enabled AWS CloudTrail to log all user/API activity for compliance and traceability.
  

Tools and Technologies:  
- Amazon S3  
- Amazon Athena  
- AWS Glue Studio  
- AWS CloudTrail  
- AWS CloudWatch  
- AWS KMS  
- IAM Role Policies  
- SQL (Athena Queries)  
- ETL Design (Visual with Governance Rules)

Deliverables:  
- End-to-end AWS analytics pipeline with monitoring, security, and governance  
- Executed SQL queries on salary trends, workforce structure, and classification comparison  
- CloudWatch dashboard and alert system  
- Glue ETL workflow with rule-based data quality filtering  
- CloudTrail audit trail and encrypted replicated S3 buckets  
- Visuals, configurations, and code captured in supporting documentation

Timeline:  
Project completed in 2 weeks, from initial design and setup through data querying, security implementation, monitoring configuration, and final documentation.

Outcome:  
The cloud-based platform successfully processed sensitive payroll data while upholding high standards for security and governance. The system delivered meaningful insights into salary distribution, operational workforce structures, and data quality. Security measures such as encryption, replication, and audit logging were fully integrated, ensuring compliance and disaster recovery readiness for future operational use.
