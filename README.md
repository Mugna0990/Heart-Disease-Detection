# Heart Disease Detection

## Overview

This project aims to Predict the presence of heart disease in patients building several models (Logistic Regression, Random Forest, XGBoost).

## Dataset

The dataset used is the "Processed Cleveland" data from the UCI Machine Learning Repository. 

**Features:**

| **Attribute** | **Description** |
|---------------|-----------------|
| `age` | Age in years |
| `sex` | Biological sex:<br>• 1 = Male<br>• 0 = Female |
| `cp` | Chest pain type:<br>• 1 = Typical angina<br>• 2 = Atypical angina<br>• 3 = Non-anginal pain<br>• 4 = Asymptomatic |
| `trestbps` | Resting blood pressure (in mm Hg) on hospital admission |
| `chol` | Serum cholesterol in mg/dl |
| `fbs` | Fasting blood sugar > 120 mg/dl:<br>• 1 = True<br>• 0 = False |
| `restecg` | Resting electrocardiographic results:<br>• 0 = Normal<br>• 1 = ST-T wave abnormality<br>• 2 = Left ventricular hypertrophy |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina:<br>• 1 = Yes<br>• 0 = No |
| `oldpeak` | ST depression induced by exercise relative to rest |
| `slope` | Slope of peak exercise ST segment:<br>• 1 = Upsloping<br>• 2 = Flat<br>• 3 = Downsloping |
| `ca` | Number of major vessels (0–3) colored by fluoroscopy |
| `thal` | Thalassemia indicator:<br>• 3 = Normal<br>• 6 = Fixed defect<br>• 7 = Reversible defect |
| `target` | Diagnosis of heart disease:<br>• 0 = No significant disease (< 50% diameter narrowing)<br>• 1 = Presence of heart disease (> 50% diameter narrowing) |

## Project Structure

The `heartDesease.ipynb` notebook contains the following sections:

- **Imports**: Loading necessary libraries.
- **Data Loading & Preprocessing**: Reading the dataset, handling missing values, converting data types, creating the target variable and splitting data.
- **Exploratory Data Analysis (EDA)**: Visualizing feature distributions and correlations.
- **Model Comparison**: Training and evaluating Logistic Regression, Random Forest and XGBoost models and comparing their test set accuracy 
- **Random Forest Model Tuning**: Using `GridSearchCV` to find optimal hyperparameters for XGBoost.
- **XGBoost Model Tuning**: Using `GridSearchCV` to find optimal hyperparameters for XGBoost.
- **Error Analysis**: Visualizing misclassified samples

## Results Summary

Based on the validation set accuracy from this run:

- **Basic Logistic Regression:** 0.8333
- **Basic Random Forest:**       0.8500
- **Basic XGBoost:**             0.8667
- **Tuned XGBoost:**             0.8667
- **Tuned Random Forest:**       0.8333
