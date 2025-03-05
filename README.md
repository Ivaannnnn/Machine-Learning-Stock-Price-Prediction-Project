# Machine-Learning-Stock-Price-Prediction-Project
# Stock Price Prediction using LSTM

## Introduction
 
 Stock price prediction is a critical task for investors, analysts, and financial professionals looking to make informed decisions in the stock market. The goal of this project is to predict future stock prices using historical price data, specifically focusing on Indofood (INDF.JK), a well-known company listed on the Indonesia Stock Exchange. In this project, we explore the use of Long Short-Term Memory (LSTM) networks, a type of recurrent neural network (RNN) designed for sequence prediction tasks. LSTM models are particularly well-suited for time-series data, such as stock prices, due to their ability to learn and remember long-term dependencies in sequential data. The project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, which provides a structured approach to data mining projects. This methodology is widely used for machine learning tasks and ensures that the project is carried out systematically, starting from business understanding all the way through to deployment.

## Objectives
- **Predict stock prices :** Using historical stock price data to forecast future prices.
- **Utilize LSTM :** Leverage LSTM models for time-series prediction to capture the sequential dependencies in stock price movements.
- **Evaluation and improvement :** Assess the performance of the model and explore avenues for future improvements, such as incorporating more features or fine-tuning the model.

## Project Overview
In this project, we use the Long Short-Term Memory (LSTM) model, a type of recurrent neural network (RNN), to predict future stock prices based on historical data. LSTM is particularly effective for time-series forecasting tasks, making it ideal for predicting stock prices, which follow sequential patterns over time. The stock price data is fetched from Yahoo Finance using the yfinance library, and we train the model on this data to make predictions on unseen future stock prices.

## Key Steps in the Project :
- **Data Collection :** Stock price data for Indofood (INDF.JK) is downloaded from Yahoo Finance.
- **Data Preprocessing :** The data is cleaned, scaled, and split into training and test sets to train the LSTM model effectively.
- **Model Development :** An LSTM model is developed to predict stock prices using the training data.
- **Model Evaluation :** The model's performance is evaluated by comparing predicted prices against actual prices, and visualizations are created to assess the accuracy of the predictions.
- **Prediction :** The trained model is used to predict future stock prices, providing insight into the expected direction of the stock's price.

# CRISP-DM Methodology

This project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, which is widely used for data science projects. The methodology ensures a structured and systematic approach to the project, which is broken down into the following six steps:

**1. Business Understanding**
The goal of the project is to predict future stock prices for Indofood (INDF.JK), a company listed on the Indonesia Stock Exchange. This prediction can help investors and analysts make informed decisions about buying, holding, or selling stocks based on expected price movements.

**2. Data Understanding**
The data for this project is obtained from Yahoo Finance using the yfinance library. The dataset consists of historical stock prices for Indofood, including the closing price. The data spans a period from 2015 to 2023.

**3. Data Preparation**
Feature Selection: Only the closing price is used as the feature to predict future stock prices.
Scaling: The data is scaled using MinMaxScaler to normalize the data between 0 and 1, which is important for the LSTM model to perform optimally.
Data Splitting: The dataset is divided into training (80%) and testing (20%) sets to train and evaluate the model's performance.

**4. Modeling**
LSTM Model: The LSTM model is chosen because it is well-suited for time-series forecasting tasks. The model consists of two LSTM layers followed by Dense layers. The model is trained to learn the patterns and dependencies in the historical stock price data.
Training: The model is trained on the training data and is validated on the test data.

**5. Evaluation**
The model's predictions are compared to the actual stock prices in the test set. The model’s performance is evaluated using visualizations that show how well the predicted prices match the real stock prices.

**6. Deployment**
Once the model is trained, it is used to predict future stock prices. The results can be plotted for better visualization. Additionally, the model can be retrained periodically using updated data to maintain its accuracy over time.

### Data Understanding

The data used in this project is historical stock price data for Indofood (INDF.JK), which is fetched using the yfinance library. The dataset includes the closing prices for the stock, which is the most commonly used indicator of a stock's price at the end of the trading day.

The data is collected from 2015-01-01 to 2023-01-01, and the following columns are included in the dataset:

- Date: The date of the stock price data.
- Open: The price of the stock when the market opened.
- High: The highest price the stock reached during the day.
- Low: The lowest price the stock reached during the day.
- Close: The price of the stock at the close of the market.
- Adj Close: The adjusted closing price, accounting for splits and dividends.
- Volume: The number of shares traded during the day.

The focus of this project is on the closing price, which is used as the target variable for prediction.

### Modeling
- LSTM Layers: The LSTM model is composed of two LSTM layers. LSTM is ideal for sequence prediction tasks, such as time-series forecasting, because it can capture long-term dependencies in data.
- Dense Layers: After the LSTM layers, dense layers are added to the model for the final output. The final dense layer outputs a single value, which is the predicted stock price.

### Training
- The model is trained using the training dataset, and the loss function used is Mean Squared Error (MSE), which is standard for regression tasks.
- Optimizer: The Adam optimizer is used, which is widely known for its efficient performance in deep learning tasks.

### Evaluation

After training the model, the predictions made by the LSTM model are compared with the actual stock prices in the test set. The results are visualized in a plot to evaluate the accuracy of the model’s predictions.

### Visualizations
- Actual Stock Price: The actual historical stock prices of Indofood (INDF.JK).
- Training Prediction: The predictions made by the model on the training dataset.
- Testing Prediction: The predictions made by the model on the testing dataset.
These visualizations help evaluate the model’s performance and provide a clear understanding of how well the model tracks the stock price over time.

## Conclusion
This project successfully predicts future stock prices using an LSTM model. By following the CRISP-DM methodology, the project systematically processed the data, built a predictive model, and evaluated its performance.

### The key steps involved
- Data Collection: Obtained historical stock price data for Indofood (INDF.JK).
- Data Preprocessing: Scaled the data and split it into training and testing sets.
- Modeling: Trained an LSTM model to predict stock prices.
- Evaluation: Compared the predicted prices to the actual stock prices and visualized the results.

The model is useful for making future predictions, but further improvements can be made by incorporating additional features, retraining the model with new data, or using more advanced models.

### Future work may involve
- **Retraining:** Using updated stock data to retrain the model periodically.
- **Feature Engineering:** Including additional features like trading volume, sentiment analysis, or technical indicators to improve prediction accuracy.
