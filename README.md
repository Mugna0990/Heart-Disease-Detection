# Heart Disease Prediction

## Overview

This project aims to predict the presence of heart disease in patients using the Cleveland heart disease dataset. It explores the data through Exploratory Data Analysis (EDA), preprocesses the data, and builds several models (Logistic Regression, Random Forest, XGBoost) to classify patients. The models are tuned using GridSearchCV and evaluated based on accuracy and other classification metrics.

## Dataset

The dataset used is the "Processed Cleveland" data from the UCI Machine Learning Repository. 

**Features:**

It contains 14 attributes:

1.  age: age in years
2.  sex: (1 = male; 0 = female)
3.  cp: chest pain type (1: typical angina, 2: atypical angina, 3: non-anginal pain, 4: asymptomatic)
4.  trestbps: resting blood pressure (in mm Hg on admission to the hospital)
5.  chol: serum cholestoral in mg/dl
6.  fbs: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
7.  restecg: resting electrocardiographic results (0: normal, 1: having ST-T wave abnormality, 2: showing probable or definite left ventricular hypertrophy)
8.  thalach: maximum heart rate achieved
9.  exang: exercise induced angina (1 = yes; 0 = no)
10. oldpeak: ST depression induced by exercise relative to rest
11. slope: the slope of the peak exercise ST segment (1: upsloping, 2: flat, 3: downsloping)
12. ca: number of major vessels (0-3) colored by flourosopy
13. thal: (3 = normal; 6 = fixed defect; 7 = reversable defect)
14. target: diagnosis of heart disease (angiographic disease status) (0: < 50% diameter narrowing, 1: > 50% diameter narrowing - corresponds to labels 1,2,3,4 in original dataset)

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
