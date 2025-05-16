# ITDS Final Project: Regression Models Analysis

## Introduction

This project explores different regression modeling techniques across three types of datasets: analytical functions, synthetic data, and real-world WWII weather data. The work demonstrates a comprehensive approach to regression analysis, from data generation to model evaluation.

## What I Did

### 1. **Analytical Functions Analysis**
- Generated data from three different mathematical functions with varying complexity
- Added realistic noise to simulate real-world data collection
- Applied and optimized various regression models:
  - Linear Regression
  - Polynomial Regression with different degrees
  - Ridge and Lasso with optimized alpha parameters
  - SVR and Random Forest models
- Visualized model performance and hyperparameter tuning results
- Found that polynomial regression performed best for these functions, with optimal degrees between 4-9

### 2. **Synthetic Multivariate Dataset Analysis**
- Created a controlled dataset using scikit-learn's `make_regression`
- Analyzed feature correlations and importance
- Tested regression models on data with known properties (10 features, 6 informative)
- Performed experiments to understand how noise levels and number of informative features affect model performance
- Visualized coefficient values to identify the most important predictors

### 3. **WWII Weather Data Analysis**
- Analyzed historical temperature data from weather stations during WWII (1940-1945)
- Explored sensor data quality and geographical temperature distributions
- Focused on station 22508 (Honolulu, Hawaii) for detailed analysis
- Created features for seasonality using sine/cosine transformations
- Built models to predict temperature based on calendar features
- Implemented a rolling window approach for time series forecasting
- Compared short-term (7-day) vs longer-term (14-day) prediction horizons
- Found that Random Forest performed best for this real-world data

### 4. **Model Comparison and Evaluation**
- Used appropriate metrics (MSE, RMSE, R²) to evaluate model performance
- Created visualizations to compare actual vs predicted values
- Analyzed how different models perform across various types of data
- Provided insights into which models work best for different data patterns

## Conclusion

This project demonstrates my ability to work with different types of data and apply appropriate regression techniques to each scenario. The analysis shows how model selection and hyperparameter tuning significantly impact prediction accuracy, and how understanding data patterns helps in choosing the right modeling approach.