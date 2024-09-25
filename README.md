# Credit Risk Analysis

## Overview of the Analysis

The purpose of this analysis is to create a machine learning model to predict the likelihood of a loan applicant being classified as either **high-risk** or **healthy**. By identifying high-risk applicants, financial institutions can make informed decisions and reduce loan defaults.

### Financial Information and Prediction Objective

The dataset used for this analysis contains financial information about loan applicants. The target variable is `loan_status`, which can take the following values:
- `0`: Healthy loan
- `1`: High-risk loan

The goal of this analysis is to predict the `loan_status` using features such as:
- Income
- Debt-to-income ratio
- Loan amount
- Credit score
- And other relevant features

### Machine Learning Process

The machine learning process consisted of the following stages:
1. **Data Preprocessing**: 
   - The dataset was loaded, and missing values were addressed.
   - The data was separated into `X` (features) and `y` (target variable).
   - The dataset was split into training and testing sets to evaluate model performance.

2. **Model Selection**:
   - The primary machine learning model used for this analysis was **Logistic Regression**. This model was chosen for its simplicity and effectiveness in binary classification problems.

3. **Model Training and Testing**:
   - The **Logistic Regression** model was trained using the training data.
   - After training, the model was evaluated on the test data using various performance metrics such as accuracy, precision, recall, and F1-score.

## Results

The results of the logistic regression model are summarized below:

* **Logistic Regression Model**:
    * **Accuracy**: 99%
    * **Precision (Class 1 - high-risk loans)**: 84%
    * **Recall (Class 1 - high-risk loans)**: 94%
    * **F1-Score**: 89%

## Summary

### Best-Performing Model:
The **Logistic Regression** model performs exceptionally well, achieving a high overall accuracy of 99%. It is especially effective at identifying high-risk loans, with a **recall of 94%** for the high-risk class (Class 1). This means that the model correctly identifies 94% of all high-risk loans, which is crucial for minimizing the risk of default.

### Importance of Predicting Class 1:
In this credit risk analysis, it is more important to correctly predict high-risk loans (`1`) than healthy loans (`0`). Missing a high-risk loan could result in financial losses due to default, so a model that prioritizes recall for high-risk loans is essential.

### Model Recommendation:
Based on the results, the **Logistic Regression** model is recommended for deployment. Its high recall score for high-risk loans ensures that the majority of risky loans are flagged, which is the primary goal of this analysis. This model offers an effective and reliable solution for credit risk assessment.

Further improvements can be made by testing additional machine learning algorithms or by fine-tuning the logistic regression model, but the current results demonstrate strong performance.
