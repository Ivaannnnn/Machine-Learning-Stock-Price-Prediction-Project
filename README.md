# Indofood Stock Price Prediction using LSTM

## 📌 Project Overview

**This project aims to predict Indofood (INDF.JK) stock prices using a Long Short-Term Memory (LSTM) neural network. The dataset is retrieved from Yahoo Finance (yfinance), and predictions are made for the next 3 years based on historical data from 2015 to 2023.**

## 📊 CRISP-DM Framework Implementation

***This project follows the CRISP-DM methodology:***

## 1️⃣ Business Understanding

**The goal is to forecast Indofood's stock price to help investors make informed decisions by analyzing historical trends.**

## 2️⃣ Data Understanding

**- Source: Yahoo Finance (yfinance)**

**- Features: Closing Price of Indofood (INDF.JK)**

**- Time Range: 2015 - 2023**

## 3️⃣ Data Preparation

**- Extract data using yfinance.**

**- Normalize stock prices using MinMaxScaler.**

**- Prepare data sequences (60-day time steps for predictions).**

## 4️⃣ Modeling

***Build an LSTM model with:***

**- 2 LSTM layers**

**- Dense layers for output**

**- Adam optimizer with MSE loss function**

**- Train the model using 80% training data & 20% testing data.**

## 5️⃣ Evaluation

***Evaluate predictions using:***

**- Mean Absolute Error (MAE)**

**- Mean Squared Error (MSE)**

**- Root Mean Squared Error (RMSE)**

**- R² Score**

## 6️⃣ Deployment

**- Generate future predictions (3 years ahead).**

**- Visualize results using Matplotlib.**

**- Store predictions in a structured DataFrame.**

## 📈 Results & Visualization

**- Comparison between actual and predicted stock prices.**

**- Future trend predictions (2023 - 2026).**
