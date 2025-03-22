******Project 1: Descriptive Analysis**
 
Project Description: Descriptive Analysis using AWS Data Analytic Platform for The City of Vancouver
Project Title: Understanding the Food and Housing 
Project Objective: This project focuses on designing and implementing a Data Analytic Platform (DAP) for the City of Vancouver to support descriptive analysis. The goal is to process and analyze data using AWS cloud services.
Project Requirements
1.	Design and Implement a Data Analytic Platform
2.	 Develop a cloud-based platform for data analytics using AWS.
3.	Implement the five-step descriptive analysis process:
•	Step 1: Data Ingestion
•	Step 2: Data Profiling
•	Step 3: Data Cleaning
•	Step 4: Data Cataloging
•	Step 5: Data Summarization
Dataset
•	Source: [City of Vancouver Open Data Portal] (https://opendata.vancouver.ca/)
Description: The dataset includes rental standards, housing statistics, zoning regulations, and occupancy rates.
Format: CSV
Data Fields:
•	Business Operator-Unique Identifier
•	Detail URL: The URL for the business.
•	Street Number: The number of the street.
•	Street Name: The name of the street.
•	Total Outstanding: The amount outstanding (likely unpaid fees or fines).
•	Total Units: The number of rental units associated with the operator.
•	Geom: Geometric representation of the property (spatial data).
•	Geo Local Area: The local area within Vancouver.
•	Geo_point_2d: Latitude and longitude coordinates.
Deliverables
•	AWS Data Analytic Platform Implementation 
•	Architecture Diagram (draw.io) 
•	Descriptive Analysis Report 
•	Screenshots of Implementation Steps 
•	AWS Cost Estimation Report.
Methodology
•	Data Collection and Preparation: The dataset attached below was prepared and downloaded from the city of Vancouver portal in CSV format for easy data ingestion and transformation.
•	Data Ingestion: Data is ingested from the portal of the City of Vancouver under Food and Housing and manually uploaded in the AWS S3 Bucket.
•	Data Profiling: Data is profiled using AWS Glue DataBrew to evaluate its content and structure while examining the quality characteristics.
•	Data Cleaning: In the same AWS Glue DataBrew, the data inconsistencies were addressed, i.e., unnesting the columns and renaming the columns.
•	Data Cataloging: Using a crawler in the AWS Glue to scan the cleaned and transformed dataset and then organize it further into a catalog based on the established metrics, i.e., Average Total Outstanding and Average Total Units.
•	Data Summarization: Using AWS Glue, a pipeline was created to process the cleaned dataset accessed from the S3 bucket.
Insights and Findings
The relationship between business operators and average total outstanding and total units was viewed, analyzed, and stored in real time for accurate record keeping.
Tools and Technologies Used
•	AWS S3: Storage for raw and processed data 
•	AWS Glue: Data Cataloging and ETL 
•	AWS Glue DataBrew: Data Cleaning
•	AWS Pricing Calculator: Cost estimation for AWS services 
•	draw.io: Architecture diagram design 
AWS Cost Estimation
Used the AWS Pricing Calculator to estimate monthly and yearly costs for running the DAP.
Deliverables
A detailed report that explained the process and why each step was taken and cost calculation for accurate record keeping and accountability.
•	AWS Data Analytic Platform Implementation 
•	Architecture Diagram-draw.io
•	Descriptive Analysis Report
•	Screenshots of Implementation Steps 
•	AWS Cost Estimation Report
•	Insights & Findings from Data Analysis

**Project Part 2: DAP platform Analysis**
Project Title: AWS Data Analytics Platform for the City of Vancouver
Project Description: This project focuses on leveraging AWS cloud services to develop a scalable Data Analytics Platform (DAP) for analyzing datasets from the City of Vancouver. The objective is to implement a structured ETL pipeline for data ingestion, transformation, validation, and visualization, ensuring accurate and actionable insights for stakeholders.
Background: Urban governance and workforce management rely on high-quality, structured data for decision-making. However, raw datasets from the City of Vancouver's open data portal often suffer from inconsistencies, missing values, and redundant records, making it challenging to extract reliable insights. The AWS-based Data Analytics Platform was developed to:
•	Automate data ingestion using AWS Glue and AWS S3.
•	Enhance data validation through AWS Glue Data Brew transformations.
•	Enable scalable analytics with AWS Athena.
•	Ensure security and compliance via AWS IAM, S3 encryption, and CloudTrail logging.
This project builds upon Project Part 1 by refining deployment procedures, establishing operational best practices, and implementing automated monitoring for ETL job failures, rollback processes, and data quality control.
Methodology: The AWS-based Data Analytics Platform was developed to:
•	Data Analysis: Utilizing AWS Glue and Amazon Athena to process and analyze large datasets efficiently.
•	Data Security: Ensuring encryption and controlled access through AWS Key Management Service (KMS).
•	Data Governance: Structuring metadata and enforcing access controls with AWS Glue Data Catalog.
•	Data Monitoring: Implementing AWS CloudWatch for job performance tracking and AWS CloudTrail for security logging.
The ETL pipeline follows a structured approach:
1.	Data Ingestion:
•	Extract data from the City of Vancouver's open data portal, specifically the Rental Standards Current Issues dataset.
•	Store raw data in Amazon S3, ensuring version control for historical tracking.
2.	Data Transformation & Cleaning: 
•	Process and clean raw datasets using AWS Glue Jobs.
•	Standardize missing values and resolve inconsistencies via AWS Glue Data Brew.
3.	Data Cataloging & Querying: 
•	Organize and register datasets in AWS Glue Data Catalog for structured metadata management.
•	Enable scalable SQL-based querying using Amazon Athena.
4.	Monitoring & Error Handling: 
•	Establish AWS CloudWatch alarms to track ETL job health and failure rates.
•	Enable AWS CloudTrail logging for comprehensive security auditing.
Tools and Technologies: The platform is built entirely on AWS services, ensuring scalability, security, and automation. The key tools used include:
•	AWS S3 – Cloud storage for raw and processed datasets.
•	AWS Glue – ETL jobs and data transformation workflows.
•	AWS Glue DataBrew – Automated data cleaning and profiling.
•	AWS Glue Data Catalog – Metadata storage for structured querying.
•	AWS Athena – Serverless querying engine for data analysis.
•	AWS CloudWatch – Monitoring, alerting, and job performance tracking.
•	AWS CloudTrail – Logging data access and security events.
Deliverables: The following key deliverables have been implemented: 
•	ETL Scripts – AWS Glue-based data extraction, transformation, and loading from the Rental Standards Current Issues dataset. 
•	Data Cleaning Pipeline – Automated data quality checks using AWS Glue Data Brew.
•	AWS Glue Data Catalog Schema – Structured metadata for seamless data discovery. 
•	Athena Query Templates – Pre-defined SQL queries for data analytics. 
•	CloudWatch & CloudTrail Logs – Real-time tracking of ETL job execution. 
Insights & Findings: Analysis of the Rental Standards Current Issues dataset revealed several key trends and actionable insights:
Business Questions Answered: 
•	What is the average total outstanding and total units of the dataset?
•	How many distinct Detail URL are there?
•	What is the min of the street number?
Data Governance & Quality Control: 
•	Implemented data validation rules to ensure consistency across different reporting periods.
•	Established access control policies via AWS IAM to restrict unauthorized modifications.
Data Monitoring Enhancements: 
•	Integrated AWS CloudWatch and CloudTrail for real-time logging and anomaly detection.
•	Set up automated alerts to flag discrepancies in rental violation trends.
ETL Performance Optimization: 
•	AWS Glue job execution times improved by 20% after performance tuning.
•	Query execution in Athena was optimized by partitioning data stored in S3.
Security & Compliance Enhancements: 
•	Implementation of IAM-based access controls ensured only authorized users could access critical datasets.
•	CloudTrail logs allowed tracking of all data modifications for regulatory compliance.
Conclusion
The AWS Data Analytics Platform successfully implemented a scalable, automated, and secure data processing pipeline for analyzing datasets from the City of Vancouver, specifically the Rental Standards Current Issues dataset. By leveraging AWS Glue and Athena the platform provides a structured approach to data management, ETL automation, and business intelligence.
Key achievements:
•	Automated data pipeline ensuring high accuracy and efficiency. 
•	Scalable architecture capable of handling large datasets with minimal overhead.
•	Real-time monitoring & logging to detect failures and trigger rollback processes.
•	Enhanced decision-making through visual analytics and trend detection.

**Project 3: Data Cleaning **
Project Title: AWS-Based Data Cleaning and Analysis for Workforce and Policy Management
Project Description: This project focuses on cleaning, analyzing, and structuring workforce and policy-related datasets using AWS cloud services. The goal is to ensure high-quality data for workforce management and policy assessment by applying data preprocessing techniques such as handling missing values, removing duplicates, standardizing formats, and validating data types. Additionally, the project aims to leverage AWS services for efficient data storage, processing, and querying to support scalable and cost-effective solutions.
Background: Organizations rely on accurate and structured data for effective decision-making. However, raw datasets often contain inconsistencies, missing values, and redundant information, making analysis difficult. By leveraging AWS Glue DataBrew, AWS S3, and AWS Athena, this project cleans and processes three datasets to facilitate efficient workforce management and policy compliance analysis. The cleaned datasets can help in:
•	Improving HR processes through structured employee information.
•	Enhancing policy enforcement by identifying patterns in policy-related data.
•	Facilitating better reporting for data-driven decision-making.
•	Reducing data errors to enhance compliance tracking and decision-making accuracy.
Dataset
This project involves three datasets:
Supervisor List Dataset (supervisor-list.csv)
•	Contains categorical data related to supervisors and their classifications.
•	Includes ten categorical features (Feature_1 to Feature_10).
•	Helps in analyzing leadership distribution and role categorization.
Workers List Dataset (workers-list.csv)
•	Contains personal and professional details of employees.
•	Fields include Name, Age, Email, Phone, Address, City, State, Zip Code, Position, and Application Date.
•	Provides insights into workforce demographics, job roles, and geographical distribution.
Policy List Dataset (policy-list.csv)
•	Contains numerical data related to organizational policies.
•	Includes ten numeric features (Feature_1 to Feature_10).
•	Supports policy assessment and compliance monitoring.

Methodology: The project follows a structured methodology for data cleaning and analysis:
1.	Data Ingestion: Upload raw datasets to AWS S3 for storage.
2.	Data Profiling: Analyze missing values, duplicates, and data types using AWS Glue DataBrew.
3.	Data Cleaning 
o	Handle missing values (imputation or removal).
o	Remove duplicate records.
o	Standardize formats (dates, numerical values, categorical values).
o	Validate and correct incorrect data types.
4.	Data Cataloging—Use AWS Glue Crawler to organize cleaned datasets.
5.	Data Summarization—Perform descriptive analytics using AWS Athena and Python (Pandas, Matplotlib) for insights.
Tools and Technologies
•	AWS S3: Cloud storage for raw and cleaned data.
•	AWS Glue DataBrew: Data cleaning and profiling.
•	AWS Glue Crawler: Automated data cataloging.
•	AWS Athena: Querying and analyzing cleaned data.
•	SQL:Querying structured data for further insights.
Deliverables
•	Cleaned datasets stored in AWS S3
•	Data cleaning and profiling reports 
•	AWS Glue DataBrew transformation scripts
•	AWS Athena queries for data analysis 
•	Insights and recommendations document 

**Project 4: Data Quality Control**
Project Title: AWS-Based Data Quality Control for Workforce and Policy Datasets
Project Description: This project focuses on implementing a Data Quality Control (DQC) framework using AWS cloud services for workforce and policy datasets. The goal is to ensure high data integrity, accuracy, and consistency by applying validation rules, anomaly detection, and automated error-handling mechanisms. The project integrates AWS services such as AWS Glue, AWS DataBrew, and AWS Athena to automate data quality checks, monitor data pipelines, and ensure compliance with data management standards.
Background: Data quality is critical for workforce and policy management, ensuring accurate decision-making and regulatory compliance. Poor data quality can lead to:
•	Inconsistent workforce records and policy enforcement.
•	Misclassification of supervisors and workers.
•	Gaps in policy documentation and outdated records.
By implementing a scalable AWS-based data quality framework, this project will standardize and clean data for more reliable workforce management and policy enforcement.
Dataset: The project uses three datasets related to workforce management and policy tracking.
1. Supervisor List Dataset (supervisor-list.csv)
•	Fields: Feature_1 - Feature_10
•	Common Issues: 
o	Inconsistent categorical values
o	Duplicate entries
o	Missing classifications
2. Workers List Dataset (workers-list.csv)
•	Fields: Name, Age, Email, Phone, Address, City, State, Zip Code, Position, Application Date
•	Common Issues: 
o	Invalid email and phone formats
o	Missing application dates
o	Duplicate employee records
3. Policy List Dataset (policy-list.csv)
•	Fields: Feature_1 - Feature_10
•	Common Issues: 
o	Incorrect policy classifications
o	Missing or outdated policy records
o	Anomalies in numerical fields
Methodology: The project follows a structured Data Quality Control (DQC) lifecycle:
1.	Data Ingestion & Storage
o	Load datasets into AWS S3.
o	Use AWS Glue Crawler to generate metadata catalogs.
2.	Data Profiling & Assessment
o	Perform profiling using AWS Glue DataBrew.
o	Identify anomalies, missing values, and inconsistencies.
3.	Data Validation & Quality Checks
o	Define validation rules (e.g., range checks, format checks, unique constraints) using AWS Glue DataBrew.
o	Implement validation rules for missing values, duplicate records, and inconsistent data formats.
4.	Error Handling & Anomaly Detection
o	Detect anomalies using AWS Data Brew’s built-in transformations.
o	Log and flag invalid records for manual review.
5.	Data Cleaning & Standardization
o	Fix common data quality issues using AWS Glue DataBrew transformations.
o	Remove duplicates and correct data types for numerical and categorical fields.
6.	Data Monitoring & Reporting
o	Generate data quality reports using AWS Athena & Amazon QuickSight.
o	Set up automated alerts for data quality issues.
Tools and Technologies
•	AWS S3 – Cloud storage for raw and processed data.
•	AWS Glue – ETL and metadata cataloging.
•	AWS Glue DataBrew – Data profiling and cleaning.
•	AWS Athena – Querying and analyzing cleaned data.
Data Quality Control Measures
To ensure high-quality data, the project implements:
•	Completeness Checks: Identifies and handles missing values.
•	Accuracy Validation: Validates employee and supervisor details.
•	Consistency Enforcement: Ensures uniform formats across datasets.
•	Anomaly Detection: Detects and removes outliers.
•	Duplicate Removal: Eliminates redundant workforce and policy records.
•	Standardization: Normalizes categorical and numerical data formats.
Deliverables
•	AWS-based Data Quality Control Framework 
•	Automated Validation and Error Handling System 
•	Data Cleaning and Transformation Scripts 
•	AWS Glue DataBrew Data Quality Reports 
Insights & Findings
•	Supervisor Dataset: Detected classification inconsistencies and corrected categorical labels.
•	Workers Dataset: Fixed missing application dates and standardized contact information.
•	Policy Dataset: Identified outdated policy records and implemented validation rules.
•	Anomaly Detection: Removed duplicate entries and flagged incorrect numerical values.
•	Overall Impact: Improved workforce and policy data reliability, enhancing compliance and decision-making.
Conclusion & Next Steps
This project successfully implemented a Data Quality Control (DQC) framework using AWS Glue and AWS DataBrew for workforce and policy datasets. Future enhancements include:
•	Automating anomaly detection using AWS machine learning models.
•	Integrating AWS Lambda for real-time validation workflows.
•	Expanding data quality monitoring using AWS CloudWatch.

![image](https://github.com/user-attachments/assets/3c63f7bf-80b4-40bf-88e1-25f463ee3af3)
