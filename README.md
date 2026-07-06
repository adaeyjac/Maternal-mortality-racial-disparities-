Empirical analysis of racial disparities in U.S. maternal mortality (2018–2024) using logistic regression and MLP models on CDC WONDER data.

# Maternal Mortality & Racial Disparities — Empirical Analysis

## Overview
This project analyzes racial disparities in U.S. maternal mortality rates 
between 2018 and 2024, examining whether race and temporal trends are 
statistically significant predictors of high mortality classification.

## Research Question
How do racial disparities and temporal trends affect maternal mortality 
rates among U.S. women between 2018 and 2024?

## Dataset
- **Source:** CDC WONDER Underlying Cause of Death Database (2018–2024)
- **ICD-10 Codes:** O00–O99 (Pregnancy, childbirth, and puerperium)
- **Filtered by:** Female sex, reproductive ages 15–49, all U.S. regions
- **Final dataset:** 42 observations across 6 racial groups and 7 years

## Key Findings
- Black women face nearly 3x higher maternal mortality than White women
- Maternal mortality peaked in 2021, an 84% increase from 2018, reflecting 
  the disproportionate impact of COVID-19
- Race alone achieved 88% classification accuracy confirming disparities 
  are deeply embedded and persistent across all years studied
- Black women show the strongest positive coefficient (1.1393) vs Asian 
  women at -1.3283 — one of the largest racial gaps identified

## Methods
- **Target Variable:** High Mortality — binary classification (above median 
  crude rate = 1, below = 0)
- **Predictor Variables:** Race (dummy encoded), Year
- **Model 1:** Logistic Regression — baseline interpretable classification
- **Model 2:** Multilayer Perceptron (MLP) — deep learning robust check
- **Evaluation:** Accuracy, AUC, Precision, Recall, Confusion Matrix
- **Split:** 80% training, 20% testing (random state 42)

## Results
| Metric | Logistic Regression | MLP |
|--------|-------------------|-----|
| Accuracy | 0.88 | 0.88 |
| AUC | 1.00 | 1.00 |
| Precision | 1.00 | 1.00 |
| Recall | 0.67 | 0.67 |

## Tools & Libraries
Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook

## Course
BUS626 Healthcare Analytics | SUNY New Paltz | Spring 2026
