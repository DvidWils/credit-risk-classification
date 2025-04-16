# Credit Risk Classification Report
---
## Overview of the Analysis

In this assignment, a machine learning model was developed to classify loans based on the categories of being healthy (0) or high-risk (1). The model used historical financial data from a peer-to-peer lending platform.

The target variable was `loan_status`, and the input features included borrower-specific data such as `loan_size`, `interest_rate`, `borrower_income`, `debt_to_income`, `num_of_accounts`, and `derogatory_marks`.

The machine learning process included:
- Loading and exploring the dataset (`lending_data.csv`).
- Splitting the data into features (`X`) and labels (`y`), where `y = loan_status`.
- Performing a train-test split.
- Scaling the features using `StandardScaler`.
- Training a logistic regression model using `LogisticRegression` from scikit-learn.
- Evaluating model performance using a confusion matrix and a classification report.

---

## Results

* **Machine Learning Model 1: Logistic Regression**
    * **Accuracy:** 99%
    * **Precision:**
        - Class `0` (Healthy Loans): 1.00
        - Class `1` (High-Risk Loans): 0.84
    * **Recall:**
        - Class `0`: 0.99
        - Class `1`: 0.99
    * **F1 Score:**
        - Class `0`: 1.00
        - Class `1`: 0.91

---

## Summary

The model predicts both healthy and high-risk loans effectively.

For the predicted healthy loans, 100% (precision of 1.00) were correctly identified as healthy. A 99% recall indicates the model rarely misses loans that are actually healthy.

For the predicted high-risk loans, 84% (precision of 0.84) were correctly identified as high-risk. A 99% recall means the model is highly effective at capturing nearly all actual high-risk loans.

Overall, this model is a reliable tool for identifying loan risk/evaluating credit risk it can greatly enhance the evaluation process for financial institution.
