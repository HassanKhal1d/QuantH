Credit Spread Forecasting Using Macroeconomic Indicators:
This project implements a complete machine learning pipeline to forecast credit spreads using engineered macroeconomic features. It emphasizes directional accuracy and robustness through time series validation, model tuning, and feature selection.

Project Overview:
Objective: Predict credit spread movements based on macroeconomic indicators

Target Variable: Credit spread (in basis points)

Core Focus: Directional accuracy (correctly predicting whether spreads go up or down)

Techniques Used: Feature engineering, regularized regression, tree-based models, stacking, cross-validation

Key Features:
Feature Engineering
A total of 25+ features were generated using:

Lag variables (1-day, 5-day, 10-day) for VIX, yields, and spread

Rolling mean and standard deviation

Daily percentage changes

Interest rate differentials

Interaction terms between macro indicators

Models Trained:
Linear Regression

Ridge Regression

Lasso Regression

Random Forest Regressor

XGBoost Regressor

Stacked Ensemble (Random Forest + XGBoost average)

Validation Strategy:
TimeSeriesSplit cross-validation (to prevent look-ahead bias)

Hyperparameter tuning with grid/random search

Feature filtering based on:

Tree feature importance threshold (≥ 0.001)

Lasso coefficients (absolute ≥ 2.0)

Ridge coefficients (absolute ≥ 3.0)

