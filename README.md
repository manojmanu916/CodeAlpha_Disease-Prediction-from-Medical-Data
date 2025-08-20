# CodeAlpha_Disease-Prediction-from-Medical-Data

Overview
This repository contains a Jupyter Notebook for building and evaluating machine learning models on three medical datasets: Heart Disease, Diabetes, and Breast Cancer. The project focuses on binary classification tasks—predicting the presence of heart disease, diabetes, or malignant breast cancer based on patient features. Models are trained and compared using standard metrics, with visualizations for performance analysis.

Key highlights from analysis:

Datasets:

Heart Disease: Likely the UCI Heart Disease dataset (~303 samples, 14 features including age, sex, chest pain type, etc.). Target: 'target' (1 = disease, 0 = no disease).

Diabetes: Likely the Pima Indians Diabetes dataset (~768 samples, 9 features including pregnancies, glucose, BMI, etc.). Target: 'Outcome' (1 = diabetes, 0 = no diabetes). Preprocessing includes replacing zeros with means for certain columns (Glucose, BloodPressure, etc.).

Breast Cancer: Likely the Wisconsin Breast Cancer dataset (~569 samples, 32 features including id, diagnosis, and various cell measurements). Target: 'diagnosis' (M = malignant/1, B = benign/0). Preprocessing drops the 'id' column and encodes diagnosis.

Features: Vary by dataset; numerical and categorical features are scaled and encoded as needed.

Target: Binary classification for all datasets.

Preprocessing: Handle missing/invalid values (e.g., zero imputation in diabetes), label encoding for categoricals (if any), feature scaling with StandardScaler, and train-test split (80/20).

Models: Logistic Regression, Random Forest Classifier (n_estimators=100), XGBoost Classifier.

Evaluation: Accuracy, Precision, Recall, F1-Score on the test set. Results are printed and visualized per dataset.

Results: Models are evaluated interactively (user chooses dataset or "all"). On standard datasets, expect accuracies around 80-95% depending on the model and data (e.g., Random Forest and XGBoost often outperform Logistic Regression). Note: Exact results depend on random splits; use cross-validation for robustness in production.
