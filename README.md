# Machine-Learning-Stock-Price-Prediction-Project
# Stock Price Prediction using LSTM

This project predicts stock prices using a Long Short-Term Memory (LSTM) neural network. The model is trained on historical stock data and can predict future stock prices. The project follows the **CRISP-DM** methodology to ensure a structured and effective approach.

## Table of Contents
- [Introduction](#introduction)
- [CRISP-DM Phases](#crisp-dm-phases)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Stock price prediction is a challenging task due to the volatile nature of the stock market. This project uses an LSTM model, which is well-suited for time series data, to predict the stock prices of Indofood (INDF.JK). The project is structured according to the **CRISP-DM** methodology, ensuring a systematic approach to data mining and machine learning.

## CRISP-DM Phases
The project follows the six phases of the **CRISP-DM** methodology:

### 1. Business Understanding
- **Objective**: Predict future stock prices to assist investors in making informed decisions.
- **Success Criteria**: The model should provide accurate predictions with low error rates (e.g., low RMSE and MAE).

### 2. Data Understanding
- **Data Source**: Historical stock data is fetched from Yahoo Finance using the `yfinance` library.
- **Data Exploration**: The dataset includes the closing prices of Indofood (INDF.JK) from 2015 to 2023.
- **Key Insights**: The data is a time series, requiring specialized models like LSTM for accurate predictions.

### 3. Data Preparation
- **Data Cleaning**: Missing values are handled (e.g., using forward fill).
- **Feature Engineering**: Only the 'Close' price is used, but additional features like moving averages or volume can be added.
- **Data Normalization**: The data is normalized to a range of [0, 1] using `MinMaxScaler`.
- **Dataset Creation**: The data is split into training (80%) and testing (20%) sets. Sequences of 60 days are used to predict the next day's price.

### 4. Modeling
- **Model Selection**: An LSTM model is chosen due to its effectiveness in handling time series data.
- **Model Architecture**: The model consists of two LSTM layers and two Dense layers.
- **Training**: The model is trained on the training dataset with 20 epochs.

### 5. Evaluation
- **Metrics**: The model's performance is evaluated using RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error).
- **Visualization**: The actual vs predicted stock prices are plotted to visually assess the model's accuracy.
- **Future Predictions**: The model predicts stock prices for the next 30 days, providing insights into future trends.

### 6. Deployment
- **Model Saving**: The trained model is saved as `lstm_stock_price_model.h5` for future use.
- **Usage**: The model can be deployed in a production environment to provide real-time stock price predictions.

## Features
- **Data Fetching**: Automatically downloads stock data using `yfinance`.
- **Preprocessing**: Normalizes data and prepares it for LSTM.
- **Model Building**: Uses a 2-layer LSTM model for prediction.
- **Training**: Trains the model on historical data.
- **Prediction**: Predicts stock prices for both training and testing datasets.
- **Visualization**: Plots actual vs predicted stock prices.
- **CRISP-DM Compliance**: Follows the CRISP-DM methodology for a structured approach.
- 
