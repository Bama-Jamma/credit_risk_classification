# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Overview of the Analysis

**Purpose of the Analysis:**
- The purpose of this analysis is to build machine learning models to predict loan statuses based on financial information provided in the dataset. The goal is to assess how well these models can predict whether a loan is "healthy" (0) or "high-risk" (1).

**Financial Information:**
- The dataset contains financial information related to loans, and the target variable is "loan_status," which indicates whether a loan is healthy (0) or high-risk (1).

**Variables and Data Distribution:**
- The target variable, "loan_status," was the variable of interest.
- To check the balance of the labels variable, we used `y.value_counts()` for the original dataset and `y_resampled.value_counts()` for the resampled dataset.

**Stages of the Machine Learning Process:**
- The analysis involved several key stages:
  1. Data preprocessing: Importing and splitting the data into training and testing sets.
  2. Building the original logistic regression model without resampling.
  3. Assessing model performance using metrics like balanced accuracy, confusion matrices, and classification reports.
  4. Resampling the training data using the RandomOverSampler to address class imbalance.
  5. Building a logistic regression model with the resampled data.
  6. Evaluating the model's performance again using the same metrics.

**Methods Used:**
- Logistic Regression: Logistic regression was employed as the machine learning algorithm to build predictive models.
- RandomOverSampler: Random oversampling was used to address class imbalance in the dataset.

## Results

### Machine Learning Model 1 (Original Logistic Regression Model):

- Balanced Accuracy: Approximately 0.952
- Precision for `0` (healthy loan): 1.00 (100%)
- Precision for `1` (high-risk loan): 0.85 (85%)
- Recall (Sensitivity) for `0` (healthy loan): 0.99 (99%)
- Recall (Sensitivity) for `1` (high-risk loan): 0.91 (91%)
- F1-score for `0` (healthy loan): 1.00 (100%)
- F1-score for `1` (high-risk loan): 0.88 (88%)

### Machine Learning Model 2 (Logistic Regression Model with Resampled Data):

- Balanced Accuracy: Approximately 0.994
- Precision for `0` (healthy loan): 1.00 (100%)
- Precision for `1` (high-risk loan): 0.84 (84%)
- Recall (Sensitivity) for `0` (healthy loan): 0.99 (99%)
- Recall (Sensitivity) for `1` (high-risk loan): 0.99 (99%)
- F1-score for `0` (healthy loan): 1.00 (100%)
- F1-score for `1` (high-risk loan): 0.91 (91%)

## Summary

The results indicate that both machine learning models, the original logistic regression model and the logistic regression model with resampled data, perform well in predicting loan statuses. However, the logistic regression model with resampled data demonstrates slightly better performance in terms of balanced accuracy, precision, and recall for both classes.

- **Model Performance:** The logistic regression model with resampled data achieves a higher balanced accuracy score, indicating its superior ability to predict both healthy and high-risk loans. It also has strong precision and recall for both classes.

- **Recommendation:** Based on the results, the logistic regression model with resampled data is recommended for predicting loan statuses. It performs exceptionally well in identifying both healthy and high-risk loans, making it a robust choice for this classification task.

- **Performance Consideration:** The performance of the model is essential, regardless of whether you want to predict healthy loans (`0`) or high-risk loans (`1`). However, the higher recall for high-risk loans (`1`) in the resampled model suggests that it may be more effective at identifying loans with a higher risk, which could be crucial for certain business decisions.

In summary, while both models perform well, the logistic regression model with resampled data appears to be the better choice due to its higher balanced accuracy and strong performance metrics for both classes.
