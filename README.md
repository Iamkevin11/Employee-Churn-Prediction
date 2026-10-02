# Employee Churn Prediction

## 📌 Project Overview

This project focuses on analyzing employee data and predicting whether an employee is likely to leave an organization.

The project includes data cleaning, exploratory data analysis (EDA), feature engineering, machine learning model development, hyperparameter tuning, and model evaluation.

## 🎯 Objectives

- Analyze employee characteristics and identify patterns related to employee turnover.
- Clean and preprocess the employee dataset.
- Explore relationships between employee satisfaction, workload, tenure, projects, salary, and churn.
- Build classification models to predict employee churn.
- Compare model performance using different evaluation metrics.
- Identify important features associated with employee leaving.

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook / Google Colab

## 📊 Dataset

The dataset contains employee information including:

- Satisfaction level
- Last evaluation
- Number of projects
- Average monthly hours
- Tenure
- Work accident
- Promotion in the last 5 years
- Department
- Salary
- Employee churn (`left`)

## 🔍 Project Workflow

### 1. Data Loading
The employee dataset is loaded using Pandas.

### 2. Data Cleaning

- Renamed and standardized column names.
- Checked for missing values.
- Identified and removed duplicate records.
- Investigated potential outliers.
- Examined the distribution of the target variable.

### 3. Exploratory Data Analysis

The project explores relationships between employee churn and factors such as:

- Satisfaction level
- Number of projects
- Monthly working hours
- Tenure
- Salary
- Department
- Promotions
- Work accidents

Visualizations include boxplots, histograms, scatterplots, bar charts, and correlation heatmaps.

### 4. Feature Engineering

Features were transformed into a format suitable for machine learning.

This includes:

- One-hot encoding of department.
- Encoding salary categories.
- Creating an `overworked` feature based on monthly working hours.
- Selecting relevant features for model training.

### 5. Machine Learning Models

The project evaluates several classification approaches, including:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

Hyperparameter tuning was performed using `GridSearchCV`.

### 6. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- Classification Report

### 7. Feature Importance

Feature importance was analyzed using:

- Decision Tree
- Random Forest
- XGBoost

This helps identify which employee attributes contribute most to the prediction of employee churn.

### 8. Final Prediction

The final XGBoost model is used to predict whether a new employee is likely to stay or leave the organization.

## 📁 Project Structure

```text
Employee-Churn-Prediction/
│
├── Employee_Churn_Prediction.ipynb
├── HR_comma_sep.csv
├── README.md
└── requirements.txt
