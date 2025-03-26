AWS Well-Architected Framework Evaluation

Project Title: Evaluation of AWS Well-Architected Framework Implementation in Cloud-Based Analytics Platform

Objective:  
To assess the design and implementation of a cloud-based analytics solution for payroll data in alignment with the AWS Well-Architected Framework. This evaluation identifies which best practices were implemented, partially applied, or omitted, and proposes improvements for future deployments.

Background:  
The City of Vancouver’s cloud-based analytics platform was developed using AWS services under the constraints of an academic lab environment (LabRole). This project evaluates the implementation against AWS’s six Well-Architected Pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability. Each pillar includes best practices drawn from AWS Academy Cloud Foundations and real-world architecture principles.

Dataset:  
The evaluation was based on system configurations and logs rather than the actual dataset. Operational patterns, encryption standards, IAM configurations, and monitoring data were analyzed instead of data content.

Methodology:

1. Pillar-Based Evaluation:  
   - Each AWS Well-Architected Pillar was broken down into a checklist of best practices.  
   - Team members conducted reviews of current configurations, service logs, and dashboard usage.  
   - Status was recorded as: Implemented, Partially Implemented, Not Implemented, or Not Applicable.

2. Evidence Collection:  
   - Metrics were sourced from AWS Glue jobs, Athena queries, CloudTrail logs, S3 configuration, and CloudWatch dashboards.  
   - Screenshots and documentation provided visual evidence for implementation status.

3. Gap Identification:  
   - Analysis included identifying features unavailable due to LabRole limitations (e.g., MFA, billing alerts).  
   - Recommendations were made for future enhancements where feasible.

Tools and Technologies:  
- Amazon S3  
- AWS Glue  
- Amazon Athena  
- AWS CloudTrail  
- AWS CloudWatch  
- IAM LabRole  
- AWS KMS  
- AWS Pricing Calculator

Deliverables:  
- Full evaluation tables for all six AWS Well-Architected Pillars  
- Summaries for each pillar outlining key achievements and gaps  
- Final reflection section identifying limitations and improvement areas  
- Visual evidence captured through AWS console screenshots

Timeline:  
Completed within one academic week during the final evaluation phase of the cloud architecture project. Review and documentation were conducted collaboratively by all team members.

Outcome:  
The platform aligned well with best practices in Security, Performance Efficiency, and Operational Excellence**, especially regarding encryption, versioning, and serverless tools. Key limitations were due to LabRole restrictions, which prevented the use of advanced IAM policies, MFA, alerting, and real billing metrics. In future implementations, enabling automated alerts, lifecycle policies, and access to AWS Config and Trusted Advisor would significantly enhance the system’s reliability, cost control, and sustainability.
