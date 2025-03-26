Data Wrangling for Academic Admissions Entity-Relationship Modeling

Project Title: Designing and Structuring Academic Admissions Data Using ER Diagrams

Objective:  
The objective of this project is to model and structure data related to academic admissions processes using Entity-Relationship Diagrams (ERDs). The goal is to establish a clean relational schema to support database design, ensuring proper linkage between applicants, programs, applications, and interviews.

Background:  
Academic institutions manage various components in the admissions workflow—from applicant submissions to program mapping and interviews. To optimize this process and support robust data handling, a normalized and well-structured ER model was designed using draw.io. This forms the basis for database implementation and analytical reporting in future stages.

Dataset:  
The data model is abstract and applies to academic admissions data. It includes entities for applicants, applications, programs, and interviews. Fields include IDs, names, submission dates, and foreign key relationships between entities.

Methodology:

1. Data Collection:  
Identified key entities involved in the admissions process based on institutional needs.  
Reviewed existing data fields typically used in admissions and interview tracking systems.

2. Data Assessment:  
Validated relationships between entities such as one-to-many (Applicants to Applications) and one-to-one (Applicants to Interviews).  
Ensured no redundant or improperly linked attributes.

3. Data Cleaning (Conceptual Level):  
Normalized entity attributes to avoid duplication.  
Assigned unique identifiers (primary keys) for each entity and mapped foreign key relationships.

4. Data Transformation:  
Constructed an ER diagram using draw.io.  
Defined the following entities and relationships:
- Applicants (Applicant ID, Applicant Name)
- Programs (Program ID, Program Name)
- Applications (Application ID, Applicant ID, Program ID, Submission Date)
- Interview (Interview ID, Applicant ID)

5. Data Consolidation:  
Ensured referential integrity among relationships by applying appropriate foreign key constraints.  
Reviewed cardinality (one-to-many and one-to-one) across entity links.

6. Documentation and Validation:  
ERD was documented visually and reviewed for accuracy and normalization.
<img width="1440" alt="ERD Diagram" src="https://github.com/user-attachments/assets/04915751-1a35-46d7-acca-5bc4a4fff794" />

Ready for use in SQL database schema creation and relational queries.

Tools and Technologies:  
- draw.io for ERD creation  
- SQL (planned use for schema and query development)

Deliverables:  
- Normalized ER diagram for academic admissions  
- Visual mapping of relationships and attributes  
- Logical foundation for implementing relational databases

Timeline:  
Completed within 1–2 days including review, diagramming, and documentation

Outcome:  
The final ER diagram provides a scalable, normalized structure for managing admissions-related data. It serves as a reference for database creation and supports future extensions such as data analytics, reporting, and student lifecycle tracking.
