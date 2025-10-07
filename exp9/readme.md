Time Series Forecasting for NIFTY-50

1. Aim

To Implement time series forecasting prediction for NIFTY-50 dataset

2. Problem Statement

Design and evaluate a Linear Regression–based model capable of accurately predicting future NIFTY 50 closing prices based on time-series data (days). The goal is to understand the trend of stock movement using a simple regression approach.

3. Deep Learning / Machine Learning Method & Description

This experiment demonstrates how a Linear Regression model can be applied to a time-series forecasting task.

Linear Regression:
Linear Regression is a supervised machine learning algorithm used to model the relationship between a dependent variable (target) and one or more independent variables (features) using a straight-line equation. It aims to find the best-fitting line that minimizes the error between predicted and actual values.

In this case, the model learns the relationship between the number of days since 2010 (feature) and the NIFTY 50 closing price (target).

4. Methods Applied to Solve the Problem

Data Collection:
Historical NIFTY 50 data was downloaded using the Yahoo Finance (yfinance) API from January 2010 to January 2022.

Data Preprocessing:

Extracted the ‘Close’ column representing the adjusted stock closing prices.

Converted the date column into a numerical format representing days since the start date for model training.

Removed missing values (if any).

Model Training:

The dataset was split into 80% training and 20% testing sets without shuffling to preserve time order.

A Linear Regression model was trained on the training set to learn the trend between Days and Close Price.

Model Evaluation:

The model was tested on the remaining 20% of data.

Performance was evaluated using Mean Squared Error (MSE).

The actual and predicted values were visualized using a line plot.

5. Results

The model achieved a Mean Squared Error (MSE) of:

6885528.931000548


The prediction plot shows that the model was able to follow the general trend of the stock price movement, although with limited precision for sharp fluctuations.

Visualization:
The plot clearly distinguishes between actual and predicted NIFTY 50 prices over time, highlighting the regression line’s ability to approximate the long-term trend.

6. Conclusion

The Linear Regression model provided a simple yet effective approach for forecasting the NIFTY 50 index trend. Although it does not capture sudden market volatility, it demonstrates the fundamental concept of regression-based stock trend analysis. The experiment validates that linear models can serve as a baseline for financial forecasting tasks and can be further improved using more advanced techniques like LSTM, ARIMA, or other deep learning models.
