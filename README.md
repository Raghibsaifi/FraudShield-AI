# FraudShield AI — Credit Card Fraud Detection

## Overview
FraudShield AI is a finance-focused machine learning project that explores credit card fraud detection using transaction data.

## Business Problem
Fraudulent transactions are rare compared with legitimate transactions. The goal is to identify suspicious activity while understanding the trade-off between detecting fraud and generating false alerts.

## Dataset
- Source: [Credit Card Fraud Detection — Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Original records: 284,807
- Records after duplicate removal: 283,726
- Missing values detected: 0

## Methodology
1. Data cleaning and duplicate removal
2. Exploratory data analysis and visualizations
3. Logistic Regression baseline model
4. Evaluation using precision, recall, F1-score, Average Precision, and ROC-AUC
5. Threshold comparison and business recommendations

## Baseline Results
- Fraud recall: 87.4%
- Fraud precision: 5.6%
- Average Precision (PR-AUC): 0.6719
- ROC-AUC: 0.9657

The baseline detected 83 of 95 fraud cases in the test set, missed 12, and falsely flagged 1,389 legitimate transactions.

## Business Insights
Threshold selection affects both the number of alerts and the proportion of alerts that are fraudulent. A practical threshold requires consideration of fraud losses, review capacity, and the cost of false positives.

## Limitations
The dataset contains anonymized features. This is an educational baseline and has not been validated for deployment in a real financial institution.

## Tools
Python, Pandas, scikit-learn, Matplotlib, Seaborn, and Kaggle Notebooks.

## Reproducibility
Open the notebook in Kaggle or a compatible Jupyter environment. Obtain the dataset from the linked source and run the notebook cells in order.

## Future Improvements
- Compare additional models
- Perform error analysis
- Evaluate threshold choices using business costs
- Explore a transaction-review dashboard
