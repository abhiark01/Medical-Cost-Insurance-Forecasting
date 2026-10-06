# Comprehensive Medical Cost Insurance Forecasting

## 📌 Project Overview

This project focuses on predicting individual medical insurance charges using Machine Learning. The goal is to build a data-driven model that can estimate annual medical insurance costs based on demographic, health, and family-related factors.

The project uses **Linear Regression** as the primary machine learning algorithm and applies exploratory data analysis, data preprocessing, categorical encoding, and feature engineering to improve prediction performance.

---

## 🎯 Problem Statement

Health insurance providers need to estimate the expected medical expenses of individuals to determine appropriate insurance premiums.

Traditional pricing methods may not fully capture relationships between factors such as age, BMI, and smoking status.

This project develops a machine learning model that predicts annual medical insurance charges using historical insurance data.

---

## 📊 Dataset

The project uses the **Medical Cost Personal Dataset**, containing **1,338 records**.

### Features

| Feature | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Gender of the individual |
| `bmi` | Body Mass Index |
| `children` | Number of dependents |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Annual medical insurance cost |

### Target Variable

`charges`

The target variable represents the individual's annual medical insurance charges.

---

## 🔍 Exploratory Data Analysis

The project performs exploratory analysis to understand the relationship between the input features and insurance charges.

Key observations include:

- Insurance charges generally increase with age.
- BMI has a positive relationship with insurance charges.
- Smoking status has a very strong relationship with medical costs.
- Individuals who smoke generally have significantly higher insurance charges.
- The combination of BMI and smoking status has an important effect on insurance costs.
- Insurance charges are right-skewed, with a small number of very high-cost cases.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

- Converted categorical variables into numerical representations.
- Encoded `sex` and `smoker`.
- Applied one-hot encoding to `region`.
- Separated features and target variable.
- Split the dataset into training and testing sets.

The dataset was divided using:

```python
test_size = 0.20
random_state = 42