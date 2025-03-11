# Machine-Learning-Stock-Price-Prediction-Project
# 📈 Stock Price Prediction using LSTM (3 Years Forecast)

This project applies **Machine Learning (LSTM)** to predict stock prices for the next **3 years** using historical data. The approach follows the **CRISP-DM methodology**.

---

## 🚀 **Project Overview**
- 📊 Uses **Long Short-Term Memory (LSTM)**, a deep learning model for time-series forecasting.
- 📈 **Predicts stock prices** for **3 years** ahead.
- 📅 **Data Source**: Yahoo Finance (`yfinance`).
- 🔍 **Evaluation**: Compares actual vs. predicted prices.

---

## 🔍 **CRISP-DM Methodology**
### **1️⃣ Business Understanding**
Predict future stock prices to support investment decisions.

### **2️⃣ Data Understanding**
- **Source**: Collected historical stock prices using `yfinance`.
- **Columns Used**: Closing price (`Close`).

### **3️⃣ Data Preparation**
- Scaled data using `MinMaxScaler` for LSTM training.
- Split data into **80% training** and **20% testing**.
- Created sequences (time steps) to train the LSTM model.

### **4️⃣ Modeling**
- **Built an LSTM model** with:
  - 2 LSTM layers
  - Dense layers for output prediction
- **Trained the model** using `Adam` optimizer and `Mean Squared Error (MSE)` loss function.

### **5️⃣ Evaluation**
- Compared **actual vs. predicted stock prices**.
- Plotted results using `matplotlib`.

### **6️⃣ Deployment**
- Future predictions for **3 years**.
- **Outputs visualization** in a stock price chart.

---
