# Maternal-mortality-racial-disparities-
Predictive modeling of regional U.S. cancer death rates using socioeconomic and demographic factors across 3,000+ counties via deep learning (MLP).
# Cancer Mortality Prediction — Socioeconomic & Demographic Factors

## Overview
This project investigates how accurately regional cancer death rates can 
be predicted using socioeconomic and demographic variables across 3,000+ 
U.S. counties using a deep neural network (MLP).

## Research Question
How accurately can regional cancer death rates be predicted using 
socioeconomic and demographic factors?

## Dataset
- **Source:** Cancer Regression Dataset (Kaggle)
- **Size:** 3,047 U.S. counties
- **Features:** median income, poverty rate, insurance type, race, 
  marital status, average annual cancer cases and deaths
- **Target Variable:** target_deathrate (cancer death rate per region)
- **Preprocessing:** null values removed, categorical variables encoded, 
  features normalized

## Methods
- **Model:** Deep Neural Network (MLP)
- **Architecture:** 3 hidden layers (100, 50, 25 neurons), ReLU activation
- **Optimizer:** Adam | **Loss Function:** MSE
- **Max Iterations:** 2,000
- **Evaluation:** R², MAE, RMSE, MSE

## Key Findings
- Median income and poverty rate showed strong multicollinearity, 
  confirming socioeconomic factors are deeply interrelated in predicting 
  cancer outcomes
- Model identified key socioeconomic drivers of regional cancer mortality 
  disparities through permutation-based feature importance

## Tools & Libraries
Python, scikit-learn, pandas, matplotlib, seaborn, Jupyter Notebook

## Team
Adaeyja Chambers, Ashley Biagini

## Course
BUS638 Deep Learning | SUNY New Paltz | Spring 2026
