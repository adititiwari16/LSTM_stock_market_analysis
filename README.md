# LSTM Stock Market Analysis and Prediction

This project aims to analyze and predict stock prices using historical data and machine learning techniques. It focuses on four major tech companies: Apple (AAPL), Google (GOOG), Microsoft (MSFT), and Amazon (AMZN). The analysis includes examining price changes, calculating moving averages, assessing daily returns, and evaluating the correlation between different stocks. Additionally, it demonstrates how to predict the closing price of a stock using a Long Short-Term Memory (LSTM) model.

## Table of Contents

- [Installation](#installation)
- [Data Collection](#data-collection)
- [Analysis](#analysis)
 - [Price Changes](#price-changes)
 - [Moving Averages](#moving-averages)
 - [Daily Returns](#daily-returns)
 - [Correlation Between Stocks](#correlation-between-stocks)
 - [Risk Assessment](#risk-assessment)
- [Stock Price Prediction](#stock-price-prediction)
- [Conclusion](#conclusion)

## Installation

To run this project, you need to have Python installed on your system. Additionally, you'll need to install the following Python libraries:

- `yfinance` for fetching historical stock data
- `pandas_datareader` for reading stock data
- `matplotlib` and `seaborn` for data visualization
- `numpy` for numerical operations
- `keras` for building the LSTM model

You can install these libraries using pip:

```bash
pip install yfinance pandas_datareader matplotlib seaborn numpy keras
```

## Data Collection

The project fetches historical stock data for AAPL, GOOG, MSFT, and AMZN using the `yfinance` library. The data includes the adjusted closing prices and trading volumes for each stock. The data is collected for a period of one year from the current date.

## Analysis

### Price Changes

The adjusted closing prices and trading volumes for each stock are plotted to visualize the price changes over time.

### Moving Averages

Moving averages for the adjusted closing prices over 10, 20, and 50 days are calculated and plotted for each stock. This helps in identifying trends in the stock prices.

### Daily Returns

The daily returns of each stock are calculated using the percentage change in the adjusted closing prices. The daily returns are then plotted, and a histogram of the daily returns is created to visualize the distribution of returns.

### Correlation Between Stocks

The daily returns of each stock are used to calculate the correlation between the stocks. This helps in understanding how the returns of different stocks are related to each other.

### Risk Assessment

The expected return and risk (standard deviation of daily returns) for each stock are calculated and plotted. This helps in assessing the risk associated with investing in each stock.

## Stock Price Prediction

An LSTM model is used to predict the closing price of AAPL. The historical closing prices are scaled and used to create sequences of 60 days of closing prices as input and the closing price of the 61st day as the target. The LSTM model is trained on this data and used to predict future closing prices.

## Conclusion

This project provides a comprehensive analysis of stock data, including price changes, moving averages, daily returns, correlations between stocks, risk assessment, and stock price prediction. The analysis helps in understanding the performance and risk associated with investing in the selected stocks and demonstrates the application of machine learning techniques in financial analysis.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
