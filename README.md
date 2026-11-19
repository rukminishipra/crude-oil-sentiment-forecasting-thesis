# Predicting Crude Oil Market Trends using Sentiment Analysis and Time Series Forecasting Techniques

Bachelor's thesis in Computer Science, Blekinge Institute of Technology (BTH), September 2024.

Authors: Skanda Mythreyi Kavi and Rukmini Shipra Sundaraneedi. Advisor: Lawrence E. Henesey.

The full report is in [`Predicting_Crude_Oil_Market_Trends_thesis.pdf`](Predicting_Crude_Oil_Market_Trends_thesis.pdf). This repository holds the report only; the source code is not included.

## Summary

The thesis studies whether sentiment from news headlines improves forecasts of the Europe Brent crude oil price compared with forecasts based on historical prices alone.

- **Data:** historical Europe Brent prices, and news headlines with dates collected by web scraping. The two sources were cleaned and aligned by date.
- **Sentiment:** each headline was scored with VADER and with TextBlob, and the scores were added to the price data as extra features.
- **Models:** ARIMA as the statistical baseline, and LSTM and GRU recurrent networks, trained first on prices only and then on prices with sentiment scores.
- **Evaluation:** RMSE, MAE, MSE, MAPE and R-squared, with hyperparameter tuning and validation-loss analysis.
- **Result:** adding sentiment improved the forecasts, and the LSTM model performed best. The figures are in chapter 5 of the report.

## Technologies

Python, BeautifulSoup and requests for data collection, VADER and TextBlob for sentiment scoring, ARIMA, LSTM and GRU networks in Keras, Matplotlib.
