# Loan Default Prediction using Machine Learning

## Project Overview

This project develops a machine learning model to predict whether a borrower is likely to default on a loan. The objective is to help financial institutions assess credit risk, improve lending decisions, and minimize financial losses.

## Problem Statement

Build a binary classification model to predict:

* **0** – No Loan Default
* **1** – Loan Default

## Dataset

The dataset contains applicant demographics, financial information, loan details, and credit history. The target variable is **Default**.

**Key Features**

* Age
* Income
* Loan Amount
* Credit Score
* Employment Duration
* Interest Rate
* Loan Term
* Debt-to-Income Ratio (DTI)
* Education
* Employment Type
* Marital Status
* Mortgage Status
* Dependents
* Loan Purpose
* Co-signer

After preprocessing and balancing, the dataset contains **59,306 records** with **18 features**.

## Project Workflow

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Handling class imbalance using undersampling
* Model training and evaluation
* Hyperparameter tuning
* Model comparison and selection
* Saving the best-performing model

## Models Used

* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier

## Results

| Model               | Test Accuracy |
| ------------------- | ------------: |
| Logistic Regression |     **68.2%** |
| Gradient Boosting   |     **68.0%** |
| Random Forest       |     **66.6%** |

Among the evaluated models, **Logistic Regression** achieved the best overall performance on the test dataset.

## Key Insights

* Loan default data is highly imbalanced, requiring class balancing before training.
* **Interest Rate** shows the strongest positive correlation with loan default.
* **Age**, **Income**, and **Months Employed** are negatively correlated with default risk.
* Hyperparameter tuning provided only marginal performance improvements.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow (optional)

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Place the dataset (`Loan_default.csv`) in the project directory.
4. Run the notebook sequentially to preprocess data, train models, evaluate performance, and generate predictions.

## Future Improvements

* Apply advanced resampling techniques such as SMOTE.
* Explore ensemble methods like XGBoost, LightGBM, and CatBoost.
* Improve feature engineering and model optimization.
* Deploy the trained model as a web application using Flask or Streamlit.

