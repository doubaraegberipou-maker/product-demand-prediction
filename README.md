# Product/Order Demand Prediction

## Overview
A beginner data science project that predicts daily order demand using historical order data, built with Python, pandas, and scikit-learn in Google Colab.

## Problem Statement
Businesses need to anticipate demand to manage resources effectively. This project explores whether historical order patterns can predict total daily order volume.

## Objective
Predict the "Target (Total orders)" column using order-related features (order type, urgency, sector, banking orders, etc.)

## Dataset
UCI Machine Learning Repository — Daily Demand Forecasting Orders dataset. 60 daily records, 13 columns (12 features + 1 target).

## Tools Used
- Python
- pandas
- matplotlib
- scikit-learn
- Google Colab

## Methodology
1. Loaded and cleaned the dataset (no missing values or duplicates found)
2. Explored demand patterns over time and by day of the week
3. Split data into features (X) and target (y)
4. Trained a Random Forest Regressor (80/20 train-test split)
5. Evaluated performance using MAE, RMSE, and R²

## Model Used
Random Forest Regressor (100 estimators)

## Results
- MAE: ~38 orders
- RMSE: ~57.5
- R²: 0.68

## Conclusion
The model performs reasonably well on typical demand days but underestimates high-demand spikes, likely due to the small dataset size. It demonstrates a complete data science workflow: cleaning, exploration, modeling, and evaluation.

## How to Run
1. Open `Product_Demand_Prediction.ipynb` in Google Colab
2. Upload `dataset.csv` when prompted
3. Run all cells in order