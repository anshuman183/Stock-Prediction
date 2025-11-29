# Stock Price Prediction with LSTM  

[![Python](https://img.shields.io/badge/Python-3.9-blue.svg)](https://www.python.org/)  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)  
 

This repository demonstrates how to build a **time-series forecasting model** using **Long Short-Term Memory (LSTM)** networks to predict the next 10 days of Apple (AAPL) stock prices.  

It combines **financial data sourcing** via APIs with **deep learning techniques** for sequence modeling, giving insights into how neural networks can be applied in financial forecasting.  

---

## Project Overview  

- **Objective**: Predict the next 10 days of Apple’s stock closing prices using past 100 days of historical data.  
- **Data Source**: [Tiingo API](https://api.tiingo.com/) (via `pandas_datareader`).  
- **Model Used**: Long Short-Term Memory (LSTM) — a recurrent neural network well-suited for time-series forecasting.  
- **Techniques**:  
  - Time Series Analysis  
  - Deep Learning (LSTM)  
  - Data Visualization  
  - API Integration  

---

## Tech Stack  

- **Python 3.x**  
- **Libraries**:  
  - `pandas` → Data preprocessing  
  - `numpy` → Numerical operations  
  - `matplotlib` → Visualization  
  - `pandas_datareader` → Fetching stock prices from Tiingo API  
  - `tensorflow / keras` → Model building & training  
  - `scikit-learn` → Data scaling & evaluation  

---

## Workflow  

1. **Data Collection**  
   - Fetch Apple stock prices using the Tiingo API.  
   - Extract closing price series for modeling.  

2. **Preprocessing**  
   - Normalize data using `MinMaxScaler`.  
   - Create sequences: **100 days input → 1 day output**.  

3. **Model Development**  
   - Define LSTM layers in Keras.  
   - Compile with Adam optimizer and MSE loss.  
   - Train model on historical stock price data.  

4. **Prediction**  
   - Forecast the **next 10 trading days**.  
   - Visualize predictions vs. actual values.  

5. **Evaluation**  
   - RMSE and error curves.  
   - Prediction trend visualization.  

---

## Key Learnings  

- Importance of **feature scaling** in neural networks.  
- **LSTM models** outperform simple RNNs for stock data.  
- Sliding window approach for **sequence preparation**.  
- Practical usage of **APIs (Tiingo)** for real datasets.  

---
