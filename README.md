# Loan Approval Prediction

A machine learning project that predicts loan approval decisions using financial and demographic data from the Loan Approval Prediction Dataset.

## Project Overview

This project implements a binary classification system to predict whether a loan application will be approved or rejected. The solution addresses class imbalance and provides insights into the key factors affecting loan approval decisions.

## Dataset

The Loan Approval Prediction Dataset contains information about loan applicants:
- `loan_id`: Unique ID for each loan application
- `no_of_dependents`: Number of dependents
- `education`: Education level (Graduate/Not Graduate)
- `self_employed`: Self-employment status (Yes/No)
- `income_annum`: Annual income
- `loan_amount`: Loan amount requested
- `loan_term`: Loan term in months
- `cibil_score`: Credit score
- `residential_assets_value`: Value of residential assets
- `commercial_assets_value`: Value of commercial assets
- `luxury_assets_value`: Value of luxury assets
- `bank_asset_value`: Value of bank assets
- `loan_status`: Target variable (Approved/Rejected)

## Methodology

1. **Data Exploration**: Analyzed distributions, correlations, and class imbalance
2. **Data Preprocessing**: Handled missing values, encoded categorical variables, and scaled features
3. **Class Imbalance Handling**: Applied SMOTE to balance the training data
4. **Model Training**: Implemented Logistic Regression, Decision Tree, and Random Forest classifiers
5. **Model Evaluation**: Compared performance using accuracy, precision, recall, F1-score, and ROC-AUC
6. **Feature Analysis**: Identified the most important features for prediction

## Results

### Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.89 | 0.88 | 0.90 | 0.89 | 0.95 |
| Decision Tree | 0.87 | 0.86 | 0.88 | 0.87 | 0.87 |
| Random Forest | 0.92 | 0.91 | 0.93 | 0.92 | 0.98 |

### Key Findings
- **Random Forest with SMOTE** performed best across all metrics
- **CIBIL Score** is the most important feature for loan approval
- **Income** and **Loan Amount** are also significant predictors
- **SMOTE** improved recall for the approved class by 15%

## Business Applications

- Automated loan application processing
- Risk assessment and credit scoring
- Reduced bias in lending decisions
- Faster loan approval turnaround times
- Improved customer experience in banking

## Installation

1. Clone this repository:
