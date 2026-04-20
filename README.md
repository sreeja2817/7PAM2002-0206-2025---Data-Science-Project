# 7PAM2002-0206-2025---Data-Science-Project
A Comparative Study of Machine Learning and Deep Learning Models for Multivariate Silver Price Prediction

# 📌 Overview
This project focuses on **Multivariate Time Series Forecasting of Silver Prices using Machine Learning and Deep Learning techniques**.

The study uses multiple financial indicators such as **Gold, Crude Oil, USD Index, and S&P 500** to model the complex and non-linear behaviour of silver prices. A comparative analysis is performed between traditional machine learning models and advanced deep learning models to evaluate their effectiveness in capturing temporal dependencies.
---

## 📊 Datasets
### Silver Dataset (Multivariate)
- Source: Yahoo Finance  
- Period: 2016 – 2026  
- Features: Silver, Gold, Crude Oil, USD Index, S&P 500  

---
## ⚙️ Workflow
1. Collected multivariate financial data (Silver, Gold, Crude Oil, USD Index, S&P 500) from Yahoo Finance  
2. Performed data cleaning, handling missing values, and setting time index  
3. Conducted EDA to analyse trends, correlations, and distributions  
4. Created sequence-based input using sliding window (60-day lookback)  
5. Trained and evaluated ML (Random Forest, XGBoost) and DL (LSTM, Tuned LSTM, CNN-LSTM, GRU) models  
6. Generated future forecasts using recursive prediction  

---

## 🤖 Models

- **Random Forest & XGBoost**
  - Used as baseline models  
  - Failed to capture temporal dependencies (negative R²)  

- **LSTM**
  - Strong performance  
  - Effectively captured sequential patterns in data  

- **Tuned LSTM**
  - Best performing model  
  - Improved accuracy through hyperparameter tuning  

- **CNN-LSTM & GRU**
  - Tested advanced architectures  
  - Did not outperform tuned LSTM  

---

## 📈 Performance Highlights

- **Tuned LSTM** → Best model (highest accuracy and generalisation)  
- **LSTM** → Good performance but slightly lower than tuned version  
- **ML models** → Poor performance due to lack of temporal modelling  

---

## 🔮 Forecast
- Used LSTM-based models for **future prediction (up to 6 months)**  
- Recursive forecasting approach applied  
- Predictions follow the overall trend with realistic variation  

---

## 🚀 Run on Google Colab
python
!pip install yfinance pandas numpy matplotlib seaborn scikit-learn tensorflow xgboost

-- Upload the .ipynb file
-- Run all cells
-- View metrics, plots, and forecast results
