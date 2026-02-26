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

