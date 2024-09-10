# Credit Risk Classification Analysis Report


## Overview of the Analysis

The purpose of this analysis is to develop machine learning models that can predict the creditworthiness of borrowers based on historical lending data from a peer-to-peer lending service. The goal is to classify borrowers as either low risk (0) or high risk (1), helping financial institutions make informed lending decisions.

### Data Overview

The dataset contains financial information such as loan size, interest rates, borrower income, total debt, and other factors like the number of accounts and derogatory marks. The target variable, loan_status, indicates whether the loan is low risk (0) or high risk (1).

**Target Variable**: loan_status
0: Low risk (75,036 instances)
1: High risk (2,500 instances)

**Features variables:** loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt.

### Machine Learning Process 
The process for building and evaluating classifier models included the following stages:

1. **Data Preprocessing:** The dataset was divided into features (X) and the target variable (y). We performed train-test splits to prepare the data for modeling.
   
2. **Model Selection:** Several machine learning models were trained and evaluated, including:
   
   **linear Models**
   - Logistic Regression
     
   **Tree-based Models**
   - Decision Tree Classifier
   - Random Forest Classifier
   - Extra Trees Classifier

   **Kernel-based Model**
   - Support Vector Machine (SVC)
     
   **Instance-based Learning**
   - k-Nearest Neighbors (kNN)
   - 
   **Ensemble Models**
   - Ada Boost Classifier
   - Gradient Boosting Classifier
   - XGBoost Classifier
   - Light GBM Classifier
     
4. Evaluation: Models were assessed using accuracy, precision, recall, F1 score, and area under the curve (AUC). Confusion matrices were used to evaluate classification performance.
   
## Results

1. **Logistic Regression**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.98
   - AUC: 0.9939
   - f1-score (Class 1): 0.91
     
2. **Decision Tree Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.85
   - AUC: 0.9493
   - f1-score (Class 1): 0.85
     
3. **Random Forest Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.85
   - Recall (Class 1): 0.89
   - AUC: 0.9937
   - f1-score (Class 1): 0.87
     
4. **Support Vector Machine (SVC)**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9936
   - f1-score (Class 1): 0.91
     
5. **k-Nearest Neighbors (kNN)**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9937
   - f1-score (Class 1): 0.91
     
6. **Extra Trees Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.85
   - Recall (Class 1): 0.87
   - AUC: 0.9679
   - f1-score (Class 1): 0.86
     
7. **Ada Boost Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9945
   - f1-score (Class 1): 0.91

8. **Gradient Boosting Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9943
   - f1-score (Class 1): 0.91

9. **XGBOOST Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9942
   - f1-score (Class 1): 0.91
     
10. **Light GBM Classifier**
   - Accuracy: 99%
   - Precision (Class 1): 0.84
   - Recall (Class 1): 0.99
   - AUC: 0.9947
   - f1-score (Class 1): 0.91
     
     
## Summary

All models achieve **99% accuracy**. **LightGBM* outperforms others slightly with the highest **AUC of 0.9947**, followed closely by **XGBoost** at 0.9942. Precision, recall, and F1-scores are consistent across models, indicating good handling of class imbalance. Both **LightGBM** and **XGBoost** are strong candidates for credit risk classification, with **LightGBM** showing marginally better performance.