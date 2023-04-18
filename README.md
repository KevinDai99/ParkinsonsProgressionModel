# Utilizing Data Science to Investigate Protein and Peptide Activity in Parkinson’s Disease

## Introduction:
Parkinson’s disease (PD) is a debilitating brain disorder that affects millions of people worldwide. The economic burden of PD is significant, with costs estimated to approach $80 billion by 2037. Unfortunately, there is currently no cure for PD, and the disease worsens over time. Research has shown that abnormal protein or peptide activity is a critical factor in the development and progression of PD. By utilizing data science, it may be possible to uncover important insights for the development of treatments that could slow the progression or even cure PD.

## Objectives:
Our primary objective is to gain a more comprehensive understanding of PD by investigating protein and peptide activity in individuals with PD and normal age-matched healthy controls. We will use data science techniques to analyze the data and identify any significant differences between the two groups.

Our secondary objective is to predict the progression of PD in patients using the Movement Disorder Society-Sponsored Revision of the Unified Parkinson’s Disease rating Scale (MDS-UPDRS). This comprehensive assessment tool measures both motor and non-motor symptoms associated with PD and can provide a measure of PD progression. By analyzing the MDS-UPDRS scores, we aim to make predictions about the disease progression in patients with PD.

## Methodology:
We will collect data on protein and peptide levels in individuals with PD and normal age-matched healthy controls using non-invasive techniques. We will also obtain MDS-UPDRS scores for patients with PD. We will then develop models to analyze the data and identify any significant differences between the two groups. We will use machine learning algorithms to make predictions about the progression of PD in patients based on their MDS-UPDRS scores.

## Data Preparation:
To achieve this objective, we downloaded the protein, peptide, and clinical data that we will work with from Kaggle. After downloading the dataset, we created a new SQLite database. We uploaded the data into the database and used the Python library sqlite3 to connect to the database and retrieve the data by executing SQL queries. Once we had the data, we performed necessary data cleaning and preprocessing steps, such as removing duplicates, handling missing values, and converting data types. Finally, we saved the cleaned data to a new CSV file using the Python library pandas.

## Expected Outcomes:
We expect to uncover significant insights into the molecular changes that occur as PD advances. We hope to identify biomarkers that could potentially be used for the early detection of PD and the development of new treatments. We also expect to make predictions about the disease progression in patients with PD that could improve patient outcomes and management.

## Conclusion:
In conclusion, this project aims to investigate protein and peptide activity in individuals with PD and normal age-matched healthy controls to gain a more comprehensive understanding of PD. By utilizing data science techniques, we hope to uncover significant insights that could lead to the development of treatments that could slow the progression or even cure PD. We believe that this research could make a significant contribution to our understanding of PD and lead to groundbreaking discoveries that could improve the lives of millions of people worldwide.


### Requirements

Data Model Implementation (25 points)
A Python script initializes, trains, and evaluates a model (10 points)

The data is cleaned, normalized, and standardized prior to modeling (5 points)

The model utilizes data retrieved from SQL or Spark (5 points)

The model demonstrates meaningful predictive power at least 75% classification accuracy or 0.80 R-squared. (5 points)

Data Model Optimization (25 points)
The model optimization and evaluation process showing iterative changes made to the model and the resulting changes in model performance is documented in either a CSV/Excel table or in the Python script itself (15 points)

Overall model performance is printed or displayed at the end of the script (10 points)

GitHub Documentation (25 points)
GitHub repository is free of unnecessary files and folders and has an appropriate .gitignore in use (10 points)

The README is customized as a polished presentation of the content of the project (15 points)

Group Presentation (25 points)
All group members speak during the presentation. (5 points)

Content, transitions, and conclusions flow smoothly within any time restrictions. (5 points)

The content is relevant to the project. (10 points)

The presentation maintains audience interest. (5 points)

This project will be evaluated against the requirements and assigned a grade according to the following table:


### Requirements 

Task Delegation

Building of Database (SQL) + Extraction into Python via sqlalchemy (Peter)

Data Cleaning - CSV join them together, Get rid of Nulls (Kevin) 

Data Exploration (Matplot Library) (Alisha)
Are there any patients that are outliers?
Statistical significance of the mean of protein abundance overtime? 

Feature Selection for Models (Kevin)
Correlation Matrix (Which features are not correlated to disease progression?)
Covariance Matrix (Which features are correlated with each other?)
Variance Threshold (Which features don’t have any variance among each other)
For Loop to test various features against standard neural archway (128, 128, 128)

Models (Linear Regression, Ensemble Learning, Neural Network)

Hyper-optimization of Models (Keras Tuner, CLF) - 1 hr 

Results - Data Visualization
What is the Mean Square Error?
Do any models outperform the other?
Are there any outliers regarding the MSE?
Summarization of results via Tableau (Alisha)

GitHub Documentation (Readme)
[Slides for Presentation ](https://docs.google.com/presentation/d/17_QldZsJaKhPdFU2Ns4lo1IzDus1Eby7Aq4LPr5zHiM/edit#slide=id.g22f87a8b3ca_10_0)













