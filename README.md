# credit_risk_classification

# Loan Status Prediction Machine Learning Project

## Overview

This machine learning project aims to predict loan statuses using logistic regression models with and without data resampling. The analysis evaluates model performance and provides insights into loan status prediction.

## Dependencies

To run this project, you need the following dependencies:

- Python (3.6+)
- Jupyter Notebook
- scikit-learn (sklearn)
- imbalanced-learn (imblearn)
- pandas
- numpy

You can install these dependencies using `pip`:

```bash
pip install jupyter scikit-learn imbalanced-learn pandas numpy

## Dataset

The dataset used in this project contains financial information related to loans. The primary target variable is "loan_status," indicating whether a loan is healthy (0) or high-risk (1).

## Analysis

### Purpose of the Analysis

The analysis serves the following purposes:

- Data preprocessing, including importing and splitting data into training and testing sets.
- Building an initial logistic regression model without resampling and assessing its performance.
- Addressing class imbalance using the RandomOverSampler technique.
- Building a logistic regression model using resampled data and evaluating its performance.

### Methods Used

- Logistic Regression: Logistic regression serves as the machine learning algorithm for building predictive models.
- RandomOverSampler: Resampling is applied to address class imbalance.

## Usage

To use this project for loan status prediction:

1. Clone this repository to your local machine.
2. Ensure you have Python and the required libraries installed (see Dependencies section).
3. Open and run the Jupyter Notebook files provided to replicate the analysis and models.

.