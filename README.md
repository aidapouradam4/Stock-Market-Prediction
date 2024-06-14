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
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/e655820d-b598-42ad-975b-fd1b895b2a55)

2. **Moving Averages**
   - Moving averages for 10, 20, and 50 days are calculated and plotted to understand the stock trends over different time periods.
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/0e541084-b4f5-4f5d-89f9-92fa8b4d38d4)

3. **Daily Returns**
   - The daily return for each stock is calculated and visualized to analyze the risk and volatility.
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/655d43cc-e31c-4cc6-b177-c9cead17abef)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/da6868df-2379-4d4a-bb2a-1594a5d2cde5)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/d420933d-7edc-4b23-b9b4-f8358fca5c5c)
  
4. **Correlation Between Stocks**
   - The correlation between the closing prices of different stocks is examined using scatter plots, pair plots, and heatmaps.
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/9f210fe4-0605-4f22-ba95-c9d8677f0748)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/a60123c5-edf1-447a-b367-55085a89b803)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/d9e73aa2-52f5-41f8-b6a7-987f6d859c29)
   
5. **Value at Risk (VaR)**
   - The Value at Risk is calculated to quantify the potential loss in value of the stocks with a certain level of confidence.
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/b810a53c-3047-44af-be6b-7b72cebe97b3)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/2e813ad0-f5ff-47be-8048-a53e8f6755b1)
   - ![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/69c99a59-31b5-4890-bdf8-1e17f5098215)

## Stock Price Prediction

An LSTM model is used to predict future stock prices. The model is trained on the historical closing prices of NVIDIA (NVDA) and then used to predict the prices for the next 300 days.

### Model Architecture

The LSTM model consists of:

- LSTM layers with dropout for regularization
- Dense layers for output prediction

The model is trained using the Adam optimizer and mean squared error loss function.

### Predictions

The predicted prices are visualized alongside the actual prices to compare the model's performance. An interactive Plotly plot is created to display the predicted prices with hover functionality to show dates.
![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/d374396f-537a-4caf-a67f-6d8c19baa6c7)
![image](https://github.com/aidapouradam4/Stock-Market-Prediction/assets/103252922/7c43057f-d557-4b51-9c58-46350af9b984)





## Future Work

- Explore the features affecting the price movements.
- Investigate the events during the time of minimum and maximum prices.
- Enhance the LSTM model with additional features and fine-tune the hyperparameters.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/aidapouradam4/stock-analysis.git

