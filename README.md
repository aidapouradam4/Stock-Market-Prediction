# Stock-Market-Prediction
This repository explores the fluctuations of four different stock share prices and develops a model to predict the price of NVIDIA stock.
# Stock Analysis and Prediction

This repository contains a comprehensive analysis of the stock market data for major tech companies, including Apple (AAPL), Google (GOOG), NVIDIA (NVDA), and Amazon (AMZN). The analysis covers historical price movements, correlations between different stocks, daily returns, moving averages, and risk assessment. Additionally, the repository includes a machine learning model for predicting future stock prices using LSTM (Long Short-Term Memory) neural networks.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Exploration](#data-exploration)
3. [Stock Price Prediction](#stock-price-prediction)
4. [Future Work](#future-work)
5. [Setup and Installation](#setup-and-installation)
6. [Usage](#usage)
7. [Results](#results)
8. [License](#license)

## Introduction

This project aims to address several fundamental questions related to stock market analysis:

- Is the price fluctuating too much or is it steady? What was the average price in the last 5 years? What were the minimum and maximum prices?
- Can the price of one stock affect another? What is the correlation between different stocks?
- What was the daily return of the stock on average?
- What was the moving average of various stocks?
- How much value do we put at risk by investing in a particular stock?
- How can we attempt to predict future stock behavior?

## Data Exploration

### Getting the Data

The stock data is fetched from Yahoo Finance using the `pandas_datareader` and `yfinance` libraries. The dataset includes the adjusted closing prices and trading volumes for the following stocks over the last year:

- Apple (AAPL)
- Google (GOOG)
- NVIDIA (NVDA)
- Amazon (AMZN)

### Analysis

1. **Stock Price Changes Over Time**
   - Historical closing prices and volume of sales are visualized to observe trends and patterns.
   
2. **Moving Averages**
   - Moving averages for 10, 20, and 50 days are calculated and plotted to understand the stock trends over different time periods.
   
3. **Daily Returns**
   - The daily return for each stock is calculated and visualized to analyze the risk and volatility.
   
4. **Correlation Between Stocks**
   - The correlation between the closing prices of different stocks is examined using scatter plots, pair plots, and heatmaps.
   
5. **Value at Risk (VaR)**
   - The Value at Risk is calculated to quantify the potential loss in value of the stocks with a certain level of confidence.

## Stock Price Prediction

An LSTM model is used to predict future stock prices. The model is trained on the historical closing prices of NVIDIA (NVDA) and then used to predict the prices for the next 300 days.

### Model Architecture

The LSTM model consists of:

- LSTM layers with dropout for regularization
- Dense layers for output prediction

The model is trained using the Adam optimizer and mean squared error loss function.

### Predictions

The predicted prices are visualized alongside the actual prices to compare the model's performance. An interactive Plotly plot is created to display the predicted prices with hover functionality to show dates.

## Future Work

- Explore the features affecting the price movements.
- Investigate the events during the time of minimum and maximum prices.
- Enhance the LSTM model with additional features and fine-tune the hyperparameters.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/stock-analysis.git

