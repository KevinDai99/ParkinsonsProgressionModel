# Predicting Parkinson's Disease Progression

## Abstract
Parkinson’s disease (PD) is a brain disorder that impairs movement, cognition, sleep, and other vital functions. Unfortunately, there is no cure- and the condition typically worsens over time. It is estimated that by 2037, nearly 1.6 million Americans will be afflicted with Parkinson's disease, resulting in an economic burden of approximately $80 billion.

Research has shown that abnormal protein  or peptide activity is a critical factor in the development and progression of this disease. By leveraging data science techniques to gain a deeper understanding of these factors, it may be possible to uncover important insights for the development of treatments that could slow the progression or even cure PD.

Our objective is to predict the progression of PD in patients by analyzing their MDS-UPDRS scores. which measure progression in patients with PD. The Movement Disorder Society-Sponsored Revision of the Unified Parkinson’s Disease rating Scale (MDS-UPDRS) is a comprehensive assessment tool that measures both motor and non-motor symptoms associated with PD.

Our team developed models using data on protein and peptide levels over time in both individuals with PD, as well as in normal age-matched healthy controls. By doing so, we aim to uncover significant insights into the molecular changes that occur as PD advances, potentially leading to a groundbreaking discovery.

## Description of the Data

1. Data Preparation: Combine the datasets (train_clinical_data.csv, train_peptides.csv, train_proteins.csv) into a single dataset using patient ID as the common key. Clean and preprocess the data to remove missing values, outliers, and other inconsistencies.
  a. The `train_clinical_data.csv` file contains information on each patient's visit, including the visit ID, patient ID, visit month, and UPDRS scores for     different assessments.

  b. The `train_peptides.csv` file contains information on the peptides measured in each patient's CSF sample. We will need to preprocess this data to           extract the relevant features for our neural network model.

  c. The `train_proteins.csv` file contains information on the proteins measured in each patient's CSF sample. This is the main data file that we will use       to train our neural network model.

## Feature Selection

| Average MSE | STD | # of Features |
|-------------|-----|---------------|
| 82          | 9   | 1080          |
| 90          | 6   | 1240          |
| 92          | 6   | 1181          |
| 92          | 7   | 1102          |
| 94          | 10  | 382           |
| 101         | 21  | 754           |

Correlation & co-variance matrix was used to select features. Cross-validation was conducted to evaluate the models. The top model has an avg of 82, although the high STD suggest that the model is overfitted and complex. 

## L2 Regularization

![image](https://user-images.githubusercontent.com/89043234/232931273-0ca49861-922d-40bd-8d6c-a20b61e46c92.png)

The top model was subjected to L2 regluarization for simplification. Lambda values between 0 - 1 were tested to determine strength. An lambda value of 1 was chosen due to tha low MSE, and standard deviation. 

## Model Training and Evaluation

![image](https://user-images.githubusercontent.com/89043234/232931572-0ddb7fd8-bf13-4542-af9f-88bd728e67f7.png)

![image](https://user-images.githubusercontent.com/89043234/232935077-f9a46b79-8ad0-4d53-a736-62156294d3fd.png)

The final model had a r2 square value of 0.65 and predicts patients with lower severity score than higher. This was expected as the dataset contains a lower frequency of patients with higher scores. This is a point for future investigation. 

## Presentation slidedeck
https://docs.google.com/presentation/d/17_QldZsJaKhPdFU2Ns4lo1IzDus1Eby7Aq4LPr5zHiM/edit#slide=id.g22f87a8b3ca_5_603












