# Mama-T-Restaurant-Regression-Analysis-Project
Tip Prediction Using Customer and Dining Attributes

🍽️ Mama T Restaurant – Tip Prediction (Regression Analysis)
Project by: Muhaly Ahmad Akinkunmi
Project Type: Supervised Machine Learning (Regression)
Notebook: Mama T tips.ipynb

📌 Project Overview

This project focuses on predicting customer tip amounts at Mama T Restaurant using structured dining and customer data.

The objective is to build and compare multiple regression models to estimate the tip based on:

Bill amount

Customer characteristics

Dining context

This project demonstrates a complete machine learning workflow, including:

Data understanding

Data cleaning

Exploratory Data Analysis (EDA)

Feature encoding

Feature scaling

Model training

Model evaluation

Prediction on new data

📊 Dataset Description

The dataset contains 744 records and the following features:

Column	Description
total_bill	Total customer bill amount
tip	Tip amount (Target Variable)
gender	Customer gender
smoker	Smoking status
day	Day of the week
time	Lunch or Dinner
size	Number of people in group
Data Types:

Numerical: total_bill, tip, size

Categorical: gender, smoker, day, time

🎯 Problem Statement

The goal is to build a supervised regression model that accurately predicts the tip amount based on customer and dining attributes.

Mathematically:

Input (X) → Customer & Dining Features
Output (y) → Tip Amount

🧹 Data Cleaning Process

The following preprocessing steps were applied:

✅ Checked dataset structure using df.info()

✅ Removed duplicate records (1 duplicate removed)

✅ Standardized categorical values (lowercase/capitalization fixes)

✅ Verified no missing values

✅ Performed exploratory data analysis (EDA)

📈 Exploratory Data Analysis (EDA)

Visualizations included:

Distribution of total bill

Distribution of tip amount

Total bill vs tip regression plot

Tip distribution by gender

Tip distribution by smoker status

Average tip by day and time

These visualizations helped understand tipping patterns and relationships between variables.

🔄 Feature Engineering
Encoding

Machine learning models require numeric input.

Categorical features were encoded using:

LabelEncoder()


Encoded columns:

gender

smoker

day

time

Feature Scaling

Features were standardized using:

StandardScaler()

🧠 Models Implemented

The following regression models were trained and compared:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Support Vector Regressor (SVR)

Gradient Boosting Regressor

📊 Model Evaluation

Evaluation metrics used:

MAE – Mean Absolute Error

RMSE – Root Mean Squared Error

R² Score – Model goodness of fit

Performance Summary
Model	R² Score
Linear Regression	0.034
Decision Tree	-0.436
Random Forest	0.082 (Best Performance)
SVR	-0.025
Gradient Boosting	0.010
🔎 Best Model:

Random Forest Regressor performed best among the tested models.

🧪 New Customer Prediction

Example prediction:

total_bill = 5000
gender = 1
smoker = 0
day = 2
time = 1
size = 4

Predicted Tip:
473.22

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab

📚 Key Learning Outcomes

Understanding regression modeling workflow

Data preprocessing techniques

Feature encoding & scaling

Model comparison using evaluation metrics

Making predictions on unseen data

End-to-end ML project structure

🚀 Future Improvements

Hyperparameter tuning

Cross-validation

Feature importance analysis

Outlier treatment

Percentage tip modeling

Deployment using Streamlit or Flask

👨‍💻 Author

Muhaly Ahmad Akinkunmi
Data Analyst | Healthcare Analyst | Machine Learning Enthusiast
