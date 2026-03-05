# Housing Price Prediction using Machine Learning

## Overview

This project investigates whether machine learning models can accurately predict housing prices based on property characteristics.

The analysis uses the **Ames Housing Dataset** (Kaggle: *House Prices – Advanced Regression Techniques*) which contains **79 explanatory variables describing residential homes**. 

The goal is to estimate the final sale price of homes using regression-based machine learning models.

---

## Models Implemented

The following models were trained and evaluated:

* Linear Regression
* Ridge Regression
* Lasso Regression
* ElasticNet
* Random Forest Regressor
* XGBoost Regressor

These models allow comparison between **linear models with regularization** and **tree-based ensemble models**. 

---

## Data Preprocessing

The dataset required several preprocessing steps:

* Missing value imputation
* Log transformation of skewed numerical variables
* One-hot encoding of categorical variables
* Feature engineering

A new feature called **`is_luxury`** was created to capture homes in the highest price percentile with luxury characteristics. 

---

## Model Evaluation

Models were evaluated using:

* Root Mean Squared Error (RMSE)
* R² score
* Prediction accuracy within 10% of actual price

Key results:

* **Lasso Regression:** R² ≈ 0.917 with strong generalization
* **Random Forest:** strong performance on typical home prices
* **XGBoost:** highest accuracy (~67.8% predictions within 10% error) 

---

## Repository Structure

```
housing-price-ml-prediction
│
├── code
│   └── housing_model.ipynb
│
├── data
│   ├── train.csv
│   └── test.csv
│
└── report
    └── housing_price_ml_report.pdf
```

---

## How to Run

1. Clone the repository

```
git clone https://github.com/YOUR_USERNAME/housing-price-ml-prediction.git
```

2. Install dependencies

```
pip install pandas numpy scikit-learn xgboost matplotlib
```

3. Run the notebook or script in the `code` folder.

---

## Key Findings

* Linear models such as **Lasso performed very well and showed strong generalization**.
* Tree-based models such as **Random Forest and XGBoost achieved the highest prediction accuracy**.
* Residual analysis revealed **heteroskedasticity and difficulty predicting luxury homes**, likely due to limited high-price observations. 

---

## Author

Yadhu Soppin
Econometrics & Economics Student
Erasmus University Rotterdam
