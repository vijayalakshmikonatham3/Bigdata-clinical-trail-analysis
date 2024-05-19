# clinical-trail-analysis-
This repo has clinical trial analysis on azure data bricks

Project Overview
This project involves the use of various big data tools and techniques to analyze clinical trial data. The project includes tasks such as system setup, data importing, preprocessing, analysis using PySpark, Spark SQL, and visualizations. Additionally, it covers advanced methods like using machine learning models for recommendations and detailed data exploration.

Table of Contents
1. System Setup
2. Dataset Explanation and Variables
3. Data Importing
4. Data Preprocessing
5. Analysis and Queries
6. Number of Studies
7. Types of Studies
8. Top Conditions
9. Top Sponsors
10. Completed Studies by Month. 
11. Further Analysis
12. Machine Learning Recommender System
13. Visualization

System Setup
1. Account Creation: Sign up for an Azure Databricks community edition account.
2. Workspace Access: Log in to the Databricks workspace.
3. Cluster Creation: Create a cluster in the Databricks workspace.
4. Notebooks Management: Create and use notebooks for writing and executing code.
5. Data Upload and Access: Upload data to the Databricks File System (DBFS).

Dataset Explanation and Variables

Clinical Trial Dataset (clinicaltrial_2023.csv)
1. ID: Unique identifier for each trial.
2. StudyType: Type of study (e.g., interventional, observational).
3. Status: Current status of the trial.
4. Conditions: Diseases or conditions being studied.
5. Interventions: Drugs or treatments used in the trial.
6. OutcomeMeasures: Primary and secondary outcome measures.
7. Sponsor: Organization sponsoring the trial.
8. StartDate: The start date of the trial.
9. EndDate: The end date of the trial.
   
Pharmaceutical Violations Dataset (pharma.csv)
1. ViolationID: Unique identifier for each recorded violation.
2. ParentCompany: Name of the parent company responsible for the violation.
3. ViolationType: Type of violation.
4. Date: Date when the violation was recorded.
5. Penalty: Financial penalty imposed for the violation.
   
Data Importing
- Data files are uploaded to DBFS, unzipped, and moved to the appropriate directories for analysis.

Data Preprocessing
- Preprocessing steps include reading and processing data using PySpark, splitting columns, and creating temporary views for SQL queries.

Analysis and Queries
1. Number of Studies
Count distinct study titles using PySpark DataFrame, RDD, and Spark SQL implementations.
2. Types of Studies
List all study types and their frequencies, ordered from most to least frequent.
3. Top Conditions
Identify the top 5 conditions with their frequencies.
4. Top Sponsors
Find the 10 most common sponsors that are not pharmaceutical companies.
5. Completed Studies by Month
Plot the number of completed studies for each month in 2023.

Further Analysis
1. Analysis of Trial Status and Duration: Evaluate the average duration of clinical trials segmented by their current status.
2. Distribution of Trials by Start Year: Quantify the number of clinical trials initiated each year.
3. Analysis of Clinical Trials by Funder Type: Examine the influence of various funder types on trial outcomes.

Machine Learning Recommender System
1. Data Preprocessing: Assign unique IDs, filter data, and split into training and test sets.
2. Model Training: Train an ALS model using different hyperparameters.
3. Model Evaluation: Evaluate the model using RMSE.
4. Exploring Recommendations: Generate and display game recommendations for users.
5. Training with Different Hyperparameters: Experiment with high-rank, more iterations, and low regularization parameters.

Visualization
Create visualizations to present data insights, including:
1. Distribution of studies by condition
2. Studies by funder type
3. Timeline of study status
