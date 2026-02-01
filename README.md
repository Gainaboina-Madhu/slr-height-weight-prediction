# slr-height-weight-prediction

# Height to Weight Prediction Using Simple Linear Regression

# 📌 Project Overview

- This project implements a Simple Linear Regression (SLR) model to predict a person’s weight based on their height.

- The goal is to understand the relationship between a single independent variable (height) and a dependent variable (weight).

# 🎯 Problem Statement

- Given a person’s height, predict their weight using a mathematical model trained on historical height–weight data.

- This is a supervised learning regression problem, where:

- Input feature: Height

- Output target: Weight

# 📊 Dataset Description

- Source: User-provided dataset

- File name: data (1).csv

- Number of features: 1

- Target variable: Weight

- Columns

- Height: Independent variable used to predict weight

- Weight: Dependent variable (actual weight)

**Data Characteristics:**

- Numeric, continuous values

- No categorical variables

- Suitable for linear regression due to direct proportional relationship

# ⚠️ Important Note:
- Prediction accuracy depends on dataset size, distribution of height values, and absence of extreme outliers.

# 🧠 Theory: Simple Linear Regression

- Simple Linear Regression models the relationship between two variables using a straight line:

- 𝑦 = 𝑚 𝑥 + 𝑐
- Where:
- y = Predicted Weight
- x = Height
- m = Slope (how much weight changes per unit height)
- c = Intercept

- The model minimizes the Mean Squared Error (MSE)

# 🛠️ Tools & Technologies Used

- Python – Programming language

- Pandas – Data loading & preprocessing

- NumPy – Numerical computations

- matplotlib – Exploratory Data Analysis (EDA)

- Scikit-learn – Linear regression model

- Pickle – Model serialization

# 🔄 Workflow of Height → Weight Prediction System

- The workflow describes how raw data turns into a working prediction model.

1️⃣ Data Collection

- The dataset (data (1).csv) contains historical height and weight values.

- Each row represents one data point:

- Height → input

- Weight → output

- 👉 This is supervised learning because the correct output (weight) is already known.

2️⃣ Data Loading

- The CSV file is loaded into the system using Pandas.

- Data is stored in a DataFrame, which allows easy manipulation and analysis.

- Why this step matters:
- The model cannot work directly with files — it needs structured data in memory.

3️⃣ Data Understanding & Separation

- The dataset is divided into:

- Independent variable (X): Height

- Dependent variable (y): Weight

- X → Height
- y → Weight


- 👉 Since only one feature is used, this is Simple Linear Regression.

4️⃣ Data Preprocessing

- In this project:

- No missing values

- No categorical data

- No normalization required (linear regression handles scale well for 1 feature)

- If the data had issues, this step would include:

- Removing null values


5️⃣ Model Selection

- Linear Regression is selected because:

- Relationship between height and weight is approximately linear

- Easy to interpret

- Suitable for beginner ML projects

- The mathematical form:

- Weight=m×Height+c
6️⃣ Model Training

- The model learns the best values of slope (m) and intercept (c).

- Training uses Ordinary Least Squares (OLS):

- Minimizes prediction error

- Reduces Mean Squared Error (MSE)


7️⃣ Model Evaluation

- The trained model is tested on the same dataset (or test data).

- Common metrics:

- MSE → average squared error

- R² score → how well the model fits the data


8️⃣ Model Saving (Serialization)

- The trained model is saved as:

- SLR_HEIGHT_2_WEIGHT.pkl

- Deployment

- Faster predictions

- Real-world usage

9️⃣ Model Loading

- The .pkl file is loaded whenever predictions are needed.

- The trained parameters (m and c) are restored.

🔟 Prediction (Inference)

- A new height value is given as input.

- The model applies the learned formula:

- Predicted Weight=m×Height+c


# 🧠 End-to-End Workflow Summary


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

# 📊 Exploratory Data Analysis (EDA): Scatter Plot

- Purpose: Understand structure, distribution, and relationship between variables.

- Scatter Plot:

- X-axis: Height

- Y-axis: Weight

**Observations:**

- Upward trend → weight increases with height

- Points roughly linear → SLR appropriate


# Conclusion:

- Positive linear relationship exists; dataset suitable for Simple Linear Regression.

<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/7a6938f9-fda6-4ebb-8c28-89d5c72cdc11" /> 
<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/d7efeab6-1469-4976-aad0-9f47bb5fbec7" />

# SLR Uses

1. Predicting Weight from Height

2. Predicting Salary from Years of Experience

3. Predicting House Price from Size

4. Predicting Test Score from Study Hours and so on..

**💡 Key point: Simple linear regression is best for straight-line relationships between one predictor and one outcome.**
