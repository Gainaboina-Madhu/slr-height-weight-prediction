# slr-height-weight-prediction

# Height to Weight Prediction Using Simple Linear Regression

# 📌 Project Overview

- This project implements a Simple Linear Regression (SLR) model to predict a person’s weight based on their height.

- The goal is to understand the relationship between a single independent variable (height) and a dependent variable (weight).

🎯 Problem Statement

Given a person’s height, predict their weight using a mathematical model trained on historical height–weight data.

This is a supervised learning regression problem, where:

Input feature: Height

Output target: Weight

📊 Dataset Description

Source: User-provided dataset

File name: data (1).csv

Number of features: 1

Target variable: Weight

Columns

Height: Independent variable used to predict weight

Weight: Dependent variable (actual weight)

Data Characteristics:

Numeric, continuous values

No categorical variables

Suitable for linear regression due to direct proportional relationship

⚠️ Important Note:
Prediction accuracy depends on dataset size, distribution of height values, and absence of extreme outliers.

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

y = Predicted Weight

x = Height

m = Slope (how much weight changes per unit height)

c = Intercept

The model minimizes the Mean Squared Error (MSE)

🛠️ Tools & Technologies Used

Python – Programming language

Pandas – Data loading & preprocessing

NumPy – Numerical computations

matplotlib – EDA

Scikit-learn – Linear regression model

Pickle – Model serialization

🔄 Workflow of Height → Weight Prediction System

Data Collection

Dataset data (1).csv contains historical height and weight values.

Supervised learning: input (Height) and output (Weight)

Data Loading

CSV file loaded using Pandas into a DataFrame for structured data.

Data Understanding & Separation

Independent variable (X): Height

Dependent variable (y): Weight

(Optional) Data Preprocessing

No missing values, no categorical data, no normalization required

If issues existed: handle nulls, outliers, or scaling

Model Selection

Linear Regression chosen because relationship is approximately linear

Model Training

Model learns slope (m) and intercept (c) using Ordinary Least Squares (OLS)

Minimizes Mean Squared Error (MSE)

Model Evaluation

Metrics: MSE, R² score

Ensures model learns a meaningful relationship

Model Saving (Serialization)

Saved as SLR_HEIGHT_2_WEIGHT.pkl

Avoids retraining for deployment or faster predictions

Model Loading

Load .pkl file whenever predictions are needed

Prediction (Inference)

New height value input → Predicted weight = m × Height + c

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

📊 Exploratory Data Analysis (EDA): Scatter Plot

Purpose: Understand structure, distribution, and relationship between variables.

Scatter Plot:

X-axis: Height

Y-axis: Weight

Observations:

Upward trend → weight increases with height

Points roughly linear → SLR appropriate

No extreme outliers

Conclusion:
Positive linear relationship exists; dataset suitable for Simple Linear Regression.

<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/7a6938f9-fda6-4ebb-8c28-89d5c72cdc11" /> <img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/d7efeab6-1469-4976-aad0-9f47bb5fbec7" />
🔹 SLR Uses

Predicting Weight from Height

Predicting Salary from Years of Experience

Predicting House Price from Size

Predicting Test Score from Study Hours

💡 Key point: Simple linear regression is best for straight-line relationships between one predictor and one outcome.
