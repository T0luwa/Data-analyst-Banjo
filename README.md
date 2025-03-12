# Data-analyst-Banjo

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
•	DetailURL: The URL for the business.
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
The relationship between business operators and average total outstanding and total units was viewed and analyzed and stored in real time for accurate record keeping.
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

![image](https://github.com/user-attachments/assets/9371b5b6-2fd6-4375-b09b-a9bf8fb5f217)
