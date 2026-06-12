# Project 02 — Machine Learning Model: Predict & Evaluate
### Heart Disease Prediction (Classification)

**Pluto Academy AI & ML Internship Program 2026**

## Problem Statement
As an ML Engineer, build, train, and evaluate a machine learning model that predicts whether a patient has heart disease, comparing 3 different classification algorithms.

## Dataset
[Heart Disease Dataset (johnsmith88) — Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

13 clinical features (age, sex, chest pain type, resting BP, cholesterol, fasting blood sugar, resting ECG, max heart rate, exercise-induced angina, ST depression, slope, number of major vessels, thalassemia) and a binary `target` (1 = disease present, 0 = absent).

> **Important:** This repo includes a sample `heart.csv` generated to match the exact schema of the Kaggle dataset so the notebook runs immediately. **Before final submission, download the real dataset from Kaggle and replace `heart.csv`**, then re-run all cells (Step 0, Option A in the notebook shows the Kaggle download commands).

## What's Included
- `Project02_ML_HeartDisease.ipynb` — full notebook with preprocessing, feature engineering, 3 trained models, evaluation, and conclusion
- `heart.csv` — sample dataset (replace with real Kaggle download before submission)

## Pipeline Summary
1. **Load & Inspect** — checked shape, dtypes, missing values, duplicates
2. **Preprocessing** — median imputation for missing values in `trestbps`, `chol`, `thalach`; categorical features already integer-encoded; `StandardScaler` applied; 80/20 stratified train/test split
3. **Feature Engineering** — correlation heatmap + Random Forest feature importances; all 13 features retained
4. **Models Trained**:
   - Logistic Regression
   - Random Forest
   - K-Nearest Neighbors (k=7)
5. **Evaluation Metrics** — Accuracy, Precision, Recall, F1 Score, comparison table + bar chart
6. **Best Model** — confusion matrix and classification report for the top-performing model, with a 5-line written conclusion

## Tools
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Google Colab

## How to Run
1. Open `Project02_ML_HeartDisease.ipynb` in Google Colab
2. (Recommended) Replace `heart.csv` with the real Kaggle dataset using the download cell in Step 0
3. Run all cells top to bottom

## Submission Checklist
- [ ] GitHub repo set to public
- [ ] Colab notebook sharing set to "Anyone with link can view"
- [ ] Real Kaggle dataset used (not the sample CSV)
- [ ] All cells run without errors, outputs visible
- [ ] Comparison table screenshot saved for the submission form
- [ ] Confusion matrix / residual plot visible for best model
- [ ] 5-line conclusion present in notebook
