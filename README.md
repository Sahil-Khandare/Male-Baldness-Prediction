# Male Baldness Prediction Using Machine Learning

A machine learning project that predicts **male baldness status (Yes/No)** using demographic, family-history, hair-loss, lifestyle, and biological features. Multiple classification algorithms are evaluated, with **XGBoost** selected as the final model.

> **Note:** The dataset used in this project is synthetic. The predictions are for educational and machine-learning demonstration purposes and should not be considered a medical diagnosis.

## Overview

Male pattern baldness can be influenced by several factors, including family history, hair-loss characteristics, lifestyle factors, and biological measurements.

This project develops a binary classification system to predict whether a patient belongs to the **baldness** or **non-baldness** category.

The project covers:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature selection
- Categorical feature encoding
- Machine learning model training
- Model comparison
- XGBoost evaluation
- Feature importance analysis
- Saving the trained model and preprocessor
- User-input-based prediction using the saved model

## Tech Stack
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib
- Jupyter Notebook
  
## Features

- Handles missing values in the dataset
- Performs exploratory data analysis
- Uses One-Hot Encoding for categorical variables
- Compares multiple ML classification algorithms
- Uses XGBoost as the final selected model
- Provides accuracy, precision, recall, F1-score and ROC-AUC evaluation
- Displays feature importance
- Saves the trained XGBoost model for future predictions
- Saves the preprocessing pipeline separately
- Provides a separate notebook for prediction without retraining the model

## Architecture / Workflow

```text
                    Dataset
                       │
                       ▼
              Data Preprocessing
                       │
                       ▼
                Feature Selection
                       │
                       ▼
                One-Hot Encoding
                       │
                       ▼
              Train ML Classifiers
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
      Logistic     Decision      Random
     Regression      Tree         Forest
          │            │            │
          └────────────┼────────────┘
                       ▼
                    XGBoost
                       │
                       ▼
               Model Evaluation
                       │
                       ▼
              Selected XGBoost
                       │
              ┌────────┴────────┐
              ▼                 ▼
       Saved XGBoost       Saved Preprocessor
           Model                  │
              │                   │
              └────────┬──────────┘
                       ▼
                 User Input
                       │
                       ▼
              Data Preprocessing
                       │
                       ▼
                 XGBoost Model
                       │
                       ▼
             Baldness Prediction
                  YES / NO

```
## Dataset & Methodology

The project uses a synthetic dataset containing 5,000 male patient records.<br>
The dataset contains demographic, family-history, hair-loss, lifestyle and biological features.<br>
Target Variable: baldness_status

## Author

Sahil Khandare <br>
Engineering Student | Software Developer | AI/ML Enthusiast
