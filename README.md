# Time Series Forecasting for Alcohol Sales 

## Project Overview
This project focuses on forecasting monthly alcohol sales using Time Series analysis. Two predictive models, Linear Regression and Random Forest, are evaluated on their forecasting accuracy. The dataset spans from January 1992 to January 2019, detailing monthly alcohol sales. The project aims to predict future sales based on past sales data, employing lag features as predictors for the models.

## Data Preprocessing
- The dataset is loaded into a pandas DataFrame with `DATE` as the index column.
- Missing values are handled, and new features (`Sales_in_last_month`, `Sales_two_months_ago`, and `Sales_three_months_ago`) are created to incorporate the time series nature of the data.
- The dataset is split into features (X) and target variable (y) arrays, reshaped for modeling.

## Models and Evaluation
Two models are evaluated:
1. **Linear Regression**: A simple model to establish a baseline performance.
2. **Random Forest Regressor**: A more complex model to capture nonlinear relationships in the data.

The models are trained on the dataset, and predictions are made for the test set. The performance of each model is evaluated using the Root Mean Squared Error (RMSE), a measure of the differences between values predicted by the model and the values observed.

## Results
- The Random Forest model outperformed the Linear Regression model, indicating its superior capability in capturing the complex patterns in the time series data.
- RMSE for Random Forest: 147.41
- RMSE for Linear Regression: 467.66

Given the lower RMSE, the Random Forest model is selected for forecasting future alcohol sales.

## Visualization
The project includes visual comparisons of the predicted sales against actual sales for both models, offering an intuitive understanding of their forecasting accuracy.

## Conclusion
This project demonstrates the application of machine learning models to time series forecasting, emphasizing the importance of feature engineering and model selection in predicting future events based on past data. The Random Forest model's superior performance suggests that ensemble methods may offer significant advantages in time series forecasting tasks.
