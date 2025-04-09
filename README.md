# Math-509-final-project
# Credit Card Fraud Detection Using Machine Learning

This repository contains a course project for MATH 509 at the University of Alberta. The project applies machine learning techniques to detect credit card fraud in a highly imbalanced dataset.

## Project Overview

Credit card fraud detection is a critical task in the financial sector due to the low occurrence but high cost of fraudulent transactions. In this project, we use various classification models and sampling strategies to build a robust fraud detection system. The dataset is highly imbalanced, with only 0.172 percent of transactions labeled as fraudulent.

We compare the performance of the following models:

- Logistic Regression  
- Random Forest  
- XGBoost  
- K-Nearest Neighbors (KNN)  
- Ensemble Voting Classifier  

Resampling techniques used include:

- SMOTE (Synthetic Minority Oversampling Technique)  
- K-Means Undersampling  

Evaluation metrics include precision, recall, F1-score, and cost-sensitive analysis.

## Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Description**: 284,807 transactions made by European cardholders in September 2013. Only 492 transactions are labeled as fraud.
- **Features**: PCA-transformed variables V1 to V28, along with Time, Amount, and Class (0 = Non-Fraud, 1 = Fraud)

Note: Most variables have been anonymized due to confidentiality.

## Methodology

### Sampling Techniques

- **SMOTE**: Generates synthetic minority class samples to balance the dataset.  
- **K-Means Undersampling**: Clusters the majority class and selects representative samples to reduce its size.

### Classification Models

- Logistic Regression  
- Random Forest  
- XGBoost  
- K-Nearest Neighbors  
- Ensemble Voting Classifier (hard voting)

### Evaluation Metrics

- Precision, Recall, F1-score  
- ROC Curves  
- Precision-Recall Curves  
- Confusion Matrix  
- Custom cost-sensitive metrics

## Key Findings

- SMOTE improves the recall of fraud detection but may increase false positives.  
- K-Means undersampling effectively reduces class imbalance while preserving majority class diversity.  
- Ensemble models provide a balanced trade-off between recall and precision.  
- Model choice should depend on application requirements (e.g., alerting vs. blocking).

## Repository Structure
