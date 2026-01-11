
# Sales Forecasting Data Science Project

## Project Overview

This project focuses on building a machine learning model to **predict future sales** using historical retail data. Accurate sales forecasts help businesses make informed decisions on **inventory management, pricing, marketing strategies, and outlet planning**.

## Problem Statement

The goal is to develop a **regression-based sales forecasting model** that can predict sales accurately, enabling businesses to optimize operations and maximize revenue.

## Solution Approach

* Preprocessed historical sales data to handle missing values and inconsistencies.
* Conducted **exploratory data analysis (EDA)** to understand trends, seasonality, and key drivers of sales.
* Engineered relevant features from product, outlet, and marketing data.
* Trained multiple regression models including **Linear Regression, Decision Trees, Random Forest, CatBoost, XGBoost, and LightGBM**.
* Optimized models with **hyperparameter tuning** to improve accuracy.
* Evaluated models using **R² score and mean squared error**.

## Data Description

* **Item Identifier:** Product code to derive item category (Food, Drink, Non-Consumables).
* **Item Weight:** Net weight of the product.
* **Item Fat Content:** Low Fat or Regular.
* **Item Visibility:** Likelihood of product being noticed in the store.
* **Item Type:** Product category (Bread, Dairy, Frozen Foods, etc.).
* **Item MRP:** Maximum retail price.
* **Outlet Identifier & Type:** Outlet details and category.
* **Outlet Establishment Year & Size:** Outlet age and size classification.
* **Outlet Location Type:** Tier 1, 2, or 3.
* **Item Outlet Sales:** Target variable, sales value.

## Findings

* Sales show **seasonality** and are influenced by pricing, product attributes, and marketing campaigns.
* Regression models achieved **R² up to 0.60**, reducing mean squared error to \~1.3M.
* Key factors influencing sales include **item visibility, pricing, outlet type, and marketing efforts**.

## Insights

* Businesses can **optimize pricing, inventory, and marketing** based on forecasted sales.
* Identifying top-performing products and key sales drivers helps **strategic outlet planning**.
* Model-driven insights improve **resource allocation and operational efficiency**.

## Model Performance

| Model    | R² Score | Notes                                                                  |
| -------- | -------- | ---------------------------------------------------------------------- |
| CatBoost | 0.60     | Best parameters: learning\_rate=0.089, max\_depth=2, n\_estimators=109 |
| XGBoost  | 0.59     | Tuned for low MSE                                                      |
| LightGBM | 0.595    | Optimized for accuracy                                                 |


### Conclusion
 Sales Forecasting (Retail / FMCG Analytics) | Self Project

Built a retail sales forecasting pipeline on 8,523 records, performing EDA, missing-value imputation, and feature engineering.

Benchmarked 9 regression models with 10-fold cross-validation, achieving up to 0.574 average CV R².

Optimized CatBoost using RandomizedSearchCV, reaching 0.598 test R² and 0.605 full-data R², and deployed via pickle.
