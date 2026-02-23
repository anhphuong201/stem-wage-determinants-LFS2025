# stem-wage-determinants-LFS2025
**Project: Determinants of Hourly Wages Among STEM Professionals**
**Project Overview**
This project applies machine learning to identify and quantify the key determinants of hourly wages among STEM professionals. The objective is twofold:
1. Build a predictive regression model with strong explanatory power.
2. Generate interpretable insights about which factors most influence wage variation.
The analysis focuses on demographic characteristics, education background, and employment-related variables to understand how structural and human capital factors contribute to earnings differences.

**Problem Statement**
Which factors most significantly influence hourly wages in STEM fields, and how much does each factor contribute to wage variation?

Understanding these drivers supports:
- Workforce planning
- Compensation benchmarking
- Policy discussions on wage equity
- Talent development strategies

**Dataset**
Source: Labor Force Survey 2025, Statistics Canada https://www150.statcan.gc.ca/n1/pub/71m0001x/71m0001x2021001-eng.htm
The dataset includes anonymized records of STEM professionals with variables such as:
- Province
- Education level
- Multiple job holder statis
- Immigration status
- Gender
- Marital status
- Family type
- Class of worker
- Union status
- Employment type (full-time/part-time, permanent/temporary)
- Firm size
- Hours worked per week
- Tenure with current employer
- Hourly earnings (target variable)
Hourly earnings were log-transformed to improve model stability and reduce skewness.

**Methodology**
1. Data Preparation
- Data cleaning and handling missing values
- Categorical encoding (One-Hot Encoding for nominal variables)
- Log transformation of hourly earnings
- Train-test split

2. Model
- Random Forest Regressor
- Implemented using a Scikit-learn pipeline
- Hyperparameter tuning via GridSearchCV

3. Evaluation Metrics
R² (Coefficient of Determination) – Measures explanatory power
Mean Absolute Error (MAE) – Average absolute prediction error
Mean Squared Error (MSE) – Penalizes larger prediction errors

**Model Performance**
R² ≈ 0.68
Low MAE and MSE relative to wage distribution
The model explains a substantial portion of wage variation, indicating that selected structural and human capital factors meaningfully contribute to earnings differences.

**Key Findings**
- Multiple job holder, Education level, Union status, Employment type are strong predictors of wage differences.
- Firm size contributes meaningfully to wage variation.
- Structural job characteristics generally explain more variance than demographic variables.
