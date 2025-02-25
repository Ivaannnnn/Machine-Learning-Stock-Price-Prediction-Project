# Machine-Learning-Stock-Price-Prediction-Project
# Stock Price Prediction using LSTM

This project predicts stock prices using a Long Short-Term Memory (LSTM) neural network. The model is trained on historical stock data and can predict future stock prices.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Stock price prediction is a challenging task due to the volatile nature of the stock market. This project uses an LSTM model, which is well-suited for time series data, to predict the stock prices of Indofood (INDF.JK).

## Features
- **Data Fetching**: Automatically downloads stock data using `yfinance`.
- **Preprocessing**: Normalizes data and prepares it for LSTM.
- **Model Building**: Uses a 2-layer LSTM model for prediction.
- **Training**: Trains the model on historical data.
- **Prediction**: Predicts stock prices for both training and testing datasets.
- **Visualization**: Plots actual vs predicted stock prices.
