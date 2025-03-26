Cost Estimation for Data Analytics Platform (DAP)

Project Title: AWS Cost Estimation for Data Analytics Platform for group 
Objective:  
To estimate the monthly and annual costs of using AWS services required for preparing, transforming, and analyzing payroll data within the City of Vancouver’s cloud-based Data Analytics Platform (DAP).

Background:  
As part of the cloud migration initiative, understanding the financial impact of running analytical workloads on AWS is essential. This cost estimation focuses on the dataset preparation phase, including data ingestion, cleaning, transformation, cataloging, and querying. The AWS Pricing Calculator was used to simulate expected usage and generate a cost forecast based on real service configurations.

Dataset:  
While the estimate does not directly involve processing live datasets, it is based on anticipated usage from payroll data including employee classifications, wage ranges, and job categories. Data volumes and processing hours were projected for cost simulation purposes.

Methodology:

1. Estimation Parameters:  
   - Services estimated: Amazon S3, AWS Glue, Amazon Athena  
   - Usage per person: 2 hours/day, 4 days (total: 8 hours/person)  
   - Team size: 4 members (32 total hours of usage)

2. Cost Calculation:  
   - Storage (S3): 40 GB of data  
   - Data processing (Glue): ETL, data profiling, cataloging  
   - Querying (Athena): On-demand analysis of processed data  
   - Calculated using AWS Pricing Calculator with North Virginia region settings

3. Pricing Model:  
   - On-demand pricing  
   - No reserved instances or spot usage considered  
   - Services configured to simulate realistic classroom/enterprise usage

Tools and Technologies:  
- AWS Pricing Calculator  
- Amazon S3  
- AWS Glue  
- Amazon Athena

Deliverables:  
- AWS cost breakdown per service  
- Monthly and annual cost estimates for individual and team use  
- Visual snapshot of pricing calculator summary  
- Justification report aligning service usage with platform design

Cost Summary:
<img width="484" alt="cost" src="https://github.com/user-attachments/assets/d6c145f2-3685-4005-94d8-ecef0204a4a9" />

Annual Cost per Person: $101.64  
Annual Team Cost (4 people): $406.56

Timeline:  
Estimation process completed within 1 working day, using current AWS pricing models and simulated workload parameters.

Outcome:  
The projected cost of running the DAP infrastructure for a team of four is approximately **$33.88/month**, ensuring a cost-effective solution for payroll analytics. This estimate helps validate the scalability of the platform while remaining aligned with municipal budget constraints.
