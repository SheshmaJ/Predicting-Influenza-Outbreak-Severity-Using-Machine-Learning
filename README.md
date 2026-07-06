# Predicting-Influenza-Outbreak-Severity-Using-Machine-Learning

# Regional Influenza Outbreak Severity Prediction for Healthcare Planning

## Overview

This project predicts influenza outbreak severity across different U.S. regions using historical influenza surveillance data from the Centers for Disease Control and Prevention (CDC). By analyzing historical influenza activity and laboratory surveillance data, the project develops machine learning regression models to forecast future influenza outbreak severity and support healthcare preparedness.

---

## Dataset

The project uses two publicly available CDC surveillance datasets:

- ILINet Dataset
- Clinical Laboratory Surveillance Dataset

  **Source:** CDC FluView Surveillance Portal  
https://gis.cdc.gov/grasp/fluview/fluportaldashboard.html

These datasets were merged to create a unified dataset containing influenza surveillance, laboratory testing, and engineered features.

---

## Objective

The objective of this project is to predict influenza positivity one week ahead (target_1wk), where target_1wk represents the percentage of laboratory-confirmed influenza-positive tests in the following week. Predicting next week's influenza positivity provides an early indication of outbreak severity and helps healthcare organizations prepare for increased influenza activity.
---

## Project Workflow

- Data Understanding
- Data Cleaning and Preprocessing
- Feature Engineering
- Feature Transformation
- Exploratory Data Analysis (EDA)
- Machine Learning Modeling
- Hyperparameter Tuning
- Model Evaluation
- R Shiny Dashboard

---

## Feature Engineering

The following features were created:

- Created lag features (lag1_percent_positive, lag1_total_specimens, lag1_total_a, lag1_total_b, and lag1_ili) to capture influenza activity from the previous week.
- Developed rolling average features (roll4_percent_positive, roll4_total_specimens, roll4_total_a, roll4_total_b, and roll4_ili) to represent recent four-week influenza trends.
- Generated change features (positive_change, specimens_change, total_a_change, total_b_change, and ili_change) to measure week-to-week changes in influenza activity.
- Calculated ratio features (a_ratio, b_ratio, and ili_patient_ratio) to describe relationships between laboratory-confirmed influenza cases and patient visits.
- Engineered seasonal features (week_sin and week_cos) to capture the cyclical pattern of influenza activity throughout the year.

---

## Exploratory Data Analysis

The project includes:

- Correlation Analysis
- Geographic Analysis
- Seasonal Analysis
- Temporal Analysis
- Persistence Analysis

---

## Machine Learning Models

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest
- XGBoost

---

## Model Evaluation

Models were evaluated using:

- RMSE
- MAE
- R² Score

---

## Technologies Used

- R
- tidyverse
- ggplot2
- caret
- glmnet
- randomForest
- xgboost
- corrplot
- R Shiny

---

## Repository Structure

```
.
├── 01_preprocessing.Rmd
├── README.md
```

---

## Project Team

**Sheshma Jaganathan** 

**Yubi Joy Quinzon**

**Celina Velazquez**

Master of Applied Data Science  
University of San Diego
