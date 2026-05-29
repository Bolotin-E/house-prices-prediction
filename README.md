# House Prices Prediction with CatBoost

🏠 Machine learning regression project focused on predicting residential property prices using feature engineering and CatBoost.


<img width="2681" height="1285" alt="House Price Analytics Dashboard" src="https://github.com/user-attachments/assets/584397aa-c535-4ed9-bd31-696e5edf180a" />


---

# Project Overview

This project explores a complete machine learning workflow for house price prediction using the Kaggle House Prices dataset.

The analysis includes:

- exploratory data analysis (EDA)
- missing value handling
- feature engineering
- categorical feature processing
- cross-validation
- model optimization
- price prediction

The final model was built using CatBoost Regressor and evaluated using cross-validation and RMSE on log-transformed target values.

---

# Dataset

Dataset: House Prices – Advanced Regression Techniques

The dataset contains residential property information including:

- lot size
- neighborhood
- house style
- year built
- quality ratings
- basement features
- garage information
- sale price

Target variable:

`SalePrice`

---

# Technologies & Tools

- Python
- Pandas
- NumPy
- CatBoost
- Scikit-Learn
- Matplotlib
- Jupyter Notebook

---

# Machine Learning Pipeline

1. Data Cleaning
2. Missing Value Treatment
3. Feature Engineering
4. Categorical Feature Processing
5. Target Transformation
6. Cross Validation
7. Model Training
8. Performance Evaluation

---

# Feature Engineering

Custom features created during the project:

### TotalSF

Combines:

- Total Basement Area
- First Floor Area
- Second Floor Area

### TotalBathrooms

Combines:

- Full Bathrooms
- Half Bathrooms
- Basement Bathrooms

### HouseAge

Measures property age:

`YrSold - YearBuilt`

### RemodAge

Measures years since remodeling:

`YrSold - YearRemodAdd`

---

# Model Architecture

Model:

`CatBoost Regressor`

Training strategy:

- categorical feature handling
- early stopping
- 5-Fold Cross Validation

---

# Model Performance

Evaluation Metric:

`RMSE (log-transformed SalePrice)`

### Validation Strategy

- 5-Fold Cross Validation
- Out-of-Fold Predictions

### Results

The CatBoost model achieved competitive performance while requiring minimal preprocessing for categorical variables.

---

# Key Features

- Regression modeling
- Feature engineering
- Cross-validation
- Target transformation
- CatBoost optimization
- Real estate price prediction

---

# Visualization

Project includes:

- feature distribution analysis
- missing value analysis
- correlation analysis
- feature importance evaluation

---

# Future Improvements

Possible next steps:

- Hyperparameter tuning
- Model stacking
- Ensemble learning
- XGBoost comparison
- LightGBM comparison

---

# Results

The project demonstrates how feature engineering and gradient boosting techniques can significantly improve predictive performance for structured tabular data.

The final solution combines domain-specific feature engineering, target transformation, and CatBoost's native handling of categorical variables to achieve strong predictive performance on residential property prices.
