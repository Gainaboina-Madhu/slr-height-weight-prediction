📊 Height to Weight Prediction Using Simple Linear Regression
Project Overview

This project implements a Simple Linear Regression (SLR) model to predict a person’s weight based on their height. The goal is to understand the relationship between a single independent variable (height) and a dependent variable (weight) and build a predictive model.

🎯 Problem Statement

Given a person’s height, predict their weight using a machine learning model trained on historical height–weight data.

Type: Supervised learning regression

Input feature: Height

Output target: Weight

📊 Dataset Description

Source: User-provided dataset

File name: data (1).csv

Number of features: 1

Target variable: Weight

Columns:

Column	Description
Height	Independent variable (predictor)
Weight	Dependent variable (target)

Data Characteristics:

Numeric, continuous values

No categorical variables

Suitable for linear regression due to direct proportional relationship

⚠ Important Note:
Prediction accuracy depends on dataset size, height distribution, and absence of extreme outliers.

🧠 Theory: Simple Linear Regression

Simple Linear Regression models the relationship between two variables using a straight line:

𝑦
=
𝑚
𝑥
+
𝑐
y=mx+c

Where:

𝑦
y = Predicted weight

𝑥
x = Height

𝑚
m = Slope (weight change per unit height)

𝑐
c = Intercept

The model minimizes the Mean Squared Error (MSE) between predicted and actual values.

🛠️ Tools & Technologies

Python – Programming language

Pandas – Data loading and preprocessing

NumPy – Numerical computations

Matplotlib – Exploratory Data Analysis (EDA)

Scikit-learn – Linear regression model

Pickle – Model serialization

🔄 Workflow: Height → Weight Prediction System

Data Collection

Historical height–weight dataset (data (1).csv)

Supervised learning: input (Height) and output (Weight)

Data Loading

CSV loaded using Pandas into a DataFrame for structured manipulation

Feature & Target Separation

Independent variable 
𝑋
X: Height

Dependent variable 
𝑦
y: Weight

Data Preprocessing (Optional)

No missing values or categorical data

No scaling required

If issues existed: handle nulls, outliers, or scaling

Model Selection

Linear Regression chosen due to linear relationship

Simple, interpretable, ideal for beginner ML projects

Model Training

Slope 
𝑚
m and intercept 
𝑐
c learned using Ordinary Least Squares (OLS)

Minimizes Mean Squared Error

Model Evaluation

Metrics:

MSE – Average squared error

R² score – Goodness of fit

Confirms the model learns a meaningful relationship

Model Saving (Serialization)

Saved as SLR_HEIGHT_2_WEIGHT.pkl for reuse

Prevents retraining and enables faster predictions

Model Loading

Load the .pkl file to restore trained parameters

Prediction (Inference)

Input a new height value → Output: Predicted weight

🧠 End-to-End Workflow Summary
Data Collection
      ↓
Data Loading
      ↓
Feature & Target Separation
      ↓
Model Selection
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Model Saving
      ↓
Model Loading
      ↓
Prediction

📊 Exploratory Data Analysis (EDA)

Purpose: Understand data structure, distribution, and relationships before modeling.

Scatter Plot Analysis:

X-axis: Height

Y-axis: Weight

Observation:

Positive upward trend → weight increases with height

Points roughly linear → SLR is appropriate

No extreme outliers observed

Conclusion:
The dataset satisfies the assumptions of Simple Linear Regression, making it a suitable modeling choice.

<img src="https://github.com/user-attachments/assets/7a6938f9-fda6-4ebb-8c28-89d5c72cdc11" width="562" alt="Scatter Plot 1" />
<img src="https://github.com/user-attachments/assets/d7efeab6-1469-4976-aad0-9f47bb5fbec7" width="562" alt="Scatter Plot 2" />
🔹 Applications of Simple Linear Regression

Predicting weight from height

Predicting salary from years of experience

Predicting house price from size

Predicting test score from study hours

💡 Key point:
Simple linear regression is ideal for straight-line relationships with one predictor and one outcome.
