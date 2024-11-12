# Credit Risk Prediction Analysis

## Overview of the Analysis

In this analysis, we developed machine learning models to predict the risk level of loan applications, classifying them as either "Healthy Loan" or "High-Risk Loan." The purpose of the analysis was to assist lenders in assessing loan applications, thereby reducing potential financial losses due to high-risk loans.

The dataset used contains financial information such as income, loan amount, debt-to-income ratio, and credit history for each loan applicant. Our goal was to predict whether a loan would be classified as high-risk based on these features.

We explored and analyzed key variables for the prediction, such as:
* Loan status (Healthy Loan or High-Risk Loan)
* Income, loan amount, and other borrower-related financial metrics
* The dataset's loan status (`value_counts` revealed a significant imbalance between Healthy Loans and High-Risk Loans).

The machine learning process included:
1. **Data Preprocessing**: Handling missing values, encoding categorical features, and scaling numerical data.
2. **Model Selection**: Implementing models like `LogisticRegression`, `Decision Tree`, and `Random Forest` to compare performance.
3. **Model Training and Evaluation**: Splitting the dataset, training each model, and evaluating accuracy, precision, and recall to gauge model effectiveness.

## Results

Below are the performance metrics (accuracy, precision, and recall) for each machine learning model:

* **Machine Learning Model 1: Logistic Regression**
    * **Accuracy**: 99%
    * **Precision (Healthy Loan)**: 1.00
    * **Recall (Healthy Loan)**: 0.99
    * **Precision (High-Risk Loan)**: 0.84
    * **Recall (High-Risk Loan)**: 0.99

* **Machine Learning Model 2: Decision Tree**
    * **Accuracy**: 99%
    * **Precision (Healthy Loan)**: 1.00
    * **Recall (Healthy Loan)**: 0.99
    * **Precision (High-Risk Loan)**: 0.84
    * **Recall (High-Risk Loan)**: 0.85

* **Machine Learning Model 3: Random Forest**
    * **Accuracy**: 99%
    * **Precision (Healthy Loan)**: 1.00
    * **Recall (Healthy Loan)**: 0.99
    * **Precision (High-Risk Loan)**: 0.85
    * **Recall (High-Risk Loan)**: 0.90

## Summary

Based on the results, the **Logistic Regression** and **Random Forest** models perform exceptionally well, with high accuracy and balanced precision and recall scores. Both models achieve 99% accuracy, but Logistic Regression slightly edges out in simplicity and interpretability.

* **Recommended Model**: Logistic Regression, due to its high performance, simplicity, and interpretability.
* **Performance Relevance**: Given the high financial stakes, accurately identifying "High-Risk Loan" cases is critical, which both Logistic Regression and Random Forest achieve with high recall (99% for Logistic Regression and 90% for Random Forest).

Overall, Logistic Regression is recommended, as it meets the project’s needs with excellent accuracy and recall for high-risk cases. If model interpretability is less important, Random Forest could also be considered for its robustness. If neither model is recommended, additional data or feature engineering may be necessary to improve performance.

