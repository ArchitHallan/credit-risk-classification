# Module 12 Report Template

## Overview of the Analysis

The aim of this analysis was to assess and build machine learning models to predict credit risk using data from a peer-to-peer lending services company. The primary focus was on the `loan_status` variable, which identifies whether a loan is healthy (0) or high-risk (1).

- **Purpose**: To predict creditworthiness of borrowers and to distinguish between healthy and high-risk loans.
- **Data**: The dataset included financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.
- **Variables**: Key variable for prediction was `loan_status`, with a significant imbalance between healthy (0) and high-risk (1) loans.
- **Machine Learning Process**: Involved data preparation, training, and evaluating models. Used `LogisticRegression` for modeling. Additionally, applied `RandomOverSampler` for resampling to address class imbalance.
- **Resampling**: Aimed to balance the dataset, ensuring equal representation of both loan types.

## Results

### Machine Learning Model 1 (Original Data)
- **Balanced Accuracy Score**: 0.9520
- **Precision (Healthy Loans - 0)**: 1.00
- **Recall (Healthy Loans - 0)**: 0.99
- **Precision (High-Risk Loans - 1)**: 0.85
- **Recall (High-Risk Loans - 1)**: 0.91

### Machine Learning Model 2 (Resampled Data)
- **Balanced Accuracy Score**: 0.9937
- **Precision (Healthy Loans - 0)**: 1.00
- **Recall (Healthy Loans - 0)**: 0.99
- **Precision (High-Risk Loans - 1)**: 0.84
- **Recall (High-Risk Loans - 1)**: 0.99

## Summary

- **Best Performing Model**: Machine Learning Model 2
- **Reason for Performance**: Model 2 demonstrates a remarkable enhancement in the recall for high-risk loans without compromising precision, which is essential for pinpointing potential defaults. The increase in balanced accuracy score also suggests a more equitable performance across both loan categories.
- **Dependence on Problem**: Deciding on the suitable model hinges on the lending company's objectives. Should the focus be on accurately pinpointing high-risk loans to mitigate default risk, Model 2 is the superior choice owing to its heightened recall for such loans.
- **Recommendation**: Given its robust performance in detecting high-risk loans—vital for curtailing financial losses in lending—Model 2 is the recommended model. Its harmonized precision and recall offer a potent tool for credit risk management.
