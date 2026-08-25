# Insurance Charges Prediction

A Machine Learning project that analyzes medical insurance data and predicts insurance charges using Linear Regression.

## 📌 Project Overview

In this project, I worked with a medical insurance dataset and followed a basic Machine Learning workflow.

The project includes:

- Exploratory Data Analysis
- Data Preprocessing
- Feature Engineering
- Correlation Analysis
- Feature Selection
- Feature Scaling
- Train-Test Split
- Linear Regression
- Model Evaluation

## 📊 Dataset

The dataset contains information about individuals and their medical insurance charges.

The original features are:

- `age`
- `sex`
- `bmi`
- `children`
- `smoker`
- `region`
- `charges`

`charges` is the target variable that the model attempts to predict.

The dataset contains **1,338 records and 7 original features**.

## 🔎 Exploratory Data Analysis

The dataset was explored to understand its structure, data types, statistical information, missing values, and relationships between variables.

Matplotlib and Seaborn were used for data visualization.

## 🧹 Data Preprocessing

The categorical features were converted into numerical representations so that they could be used by Machine Learning algorithms.

The preprocessing included:

- Checking missing values
- Encoding categorical variables
- One-hot encoding
- Creating a cleaned dataset

## ⚙️ Feature Engineering

A new feature called `BMI_Category` was created from the BMI feature.

BMI was categorized into:

- Underweight
- Normal
- Overweight
- Obese

The BMI categories were then converted into numerical features.

## 📈 Correlation & Feature Selection

Correlation analysis was performed between the features and the target variable `charges`.

A threshold was used for basic feature selection:

```text
|Correlation| < 0.05 → Drop Feature
|Correlation| ≥ 0.05 → Accept Feature
