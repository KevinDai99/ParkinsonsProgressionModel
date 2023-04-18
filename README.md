# Predicting Parkinson's Disease Progression

# Abstract
Parkinson’s disease (PD) is a brain disorder that impairs movement, cognition, sleep, and other vital functions. Unfortunately, there is no cure- and the condition typically worsens over time. It is estimated that by 2037, nearly 1.6 million Americans will be afflicted with Parkinson's disease, resulting in an economic burden of approximately $80 billion.

Research has shown that abnormal protein  or peptide activity is a critical factor in the development and progression of this disease. By leveraging data science techniques to gain a deeper understanding of these factors, it may be possible to uncover important insights for the development of treatments that could slow the progression or even cure PD.

Our objective is to predict the progression of PD in patients by analyzing their MDS-UPDRS scores. which measure progression in patients with PD. The Movement Disorder Society-Sponsored Revision of the Unified Parkinson’s Disease rating Scale (MDS-UPDRS) is a comprehensive assessment tool that measures both motor and non-motor symptoms associated with PD.

Our team developed models using data on protein and peptide levels over time in both individuals with PD, as well as in normal age-matched healthy controls. By doing so, we aim to uncover significant insights into the molecular changes that occur as PD advances, potentially leading to a groundbreaking discovery.

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

Models (Linear Regression, Ensemble Learning, Neural Network) (Kevin and Sambulo)

Hyper-optimization of Models (Keras Tuner, CLF) - 1 hr 

Results - Data Visualization
What is the Mean Square Error?
Do any models outperform the other?
Are there any outliers regarding the MSE?
Summarization of results via Tableau (Alisha)

GitHub Documentation (Readme)


## Presentation slidedeck
https://docs.google.com/presentation/d/17_QldZsJaKhPdFU2Ns4lo1IzDus1Eby7Aq4LPr5zHiM/edit#slide=id.g22f87a8b3ca_5_603












