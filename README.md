# Short-Term Stock Return Prediction Using Machine Learning
Machine learning project that integrates Alpaca API and Yahoo Finance data to engineer market features and predict 5-day forward returns for four publicly traded stocks.

# Executive Summary

This project asks and answers the question of how well a machine learning model, in our case a Random Forest, predicts 5-day forward short-term returns for the S&P 500 and 3 other individual stocks. It uses the Alpaca API and the Yahoo Finance package to obtain S&P 500 data stretching back to January 1st, 2000. The Alpaca API data is used for the NVIDIA, Johnson & Johnson, and Amazon stocks from January 1st, 2018, until February, 18 2016.

The result of the models show that they have limited predictive power when forecasting 5-day returns. This result is consistent with the market theories and proves that just using historical numerical data is extremely limited.



## Data 

### S&P (500) (SPY)

- Time Period: 2000-2026 
- Observations: 6760 daily obervations
- Variables: 11 predictors
- Target Variable: 5-day forward return

### NVIDA (NVDA)

- Time Period: 2018-2026 
- Observations: 2042 daily obervations
- Variables: 11 predictors
- Target Variable: 5-day forward return

### Johnson & Johnson (JNJ)

- Time Period: 2018-2026 
- Observations: 2042 daily obervations
- Variables: 11 predictors
- Target Variable: 5-day forward return

### Amazon (AMZN)

- Time Period: 2018-2026 
- Observations: 2042 daily obervations
- Variables: 11 predictors
- Target Variable: 5-day forward return



## Explanatory Variables

### Total Variables Used in Model: 11

### Momentum Features:

- 1_day_return
- 3_day_return 
- 5_day_return

Captures daily percentage returns over 1-day, 3-day, and 5-days. This is used to capture momentum trends. 


### Intraday Price Behavior:

- daily_range
- gap

Daily range measures difference between the day's high and low and the gap variable measures the day's volatility.


### Trend Indicators:

- moving_average_7
- moving_average_30 
- close_vs_moving_average_7
- close_vs_moving_average_30

Moving_average_7 and Moving_average_30 represent 7-day and 30-day rolling averages, while close_vs_moving_average_7 and close_vs_moving_average_30 indicate short-term trends and any trend reversals over the past 30 days.


### Volume Measures:

- volume_change

Volume_Change variable is the daily percentage change in trading volume.

### Volatility Measures:

- vol_10
- vol_20

These variables are the rolling standard deviations of returns over 10 and 20 days, respectively, capturing short-term and long-term volatility.

### Market Sentiment:

- vix

VIX, also known as the fear index, measures the expected volatility of stocks over the next 30 days. VIX is used here for sentiment analysis, and it is the closest available variable for this project.

### Target Variable:

- target

The target variable is the percentage return over the next 5 days, chosen to reduce noise and maximize accuracy.

