# Bitcoin Price Prediction — ML Model with Feature Engineering

> **Published Research** · IEEE · PES University, Bengaluru

## Overview

Price prediction module from the Bitcoin Investopedia project, published in IEEE. Predicts next-day Bitcoin closing price using real-time scraped data and engineered technical indicators.

Three models were trained — LSTM, SVR, and Linear Regression (SGD). **Linear Regression achieved 90.56% accuracy**, outperforming LSTM (76.8%) and SVR (84%).

## My Contribution
- Real-time web scraping of Bitcoin transaction data (bitinfocharts.com)
- OHLC data collection and preprocessing (Aug 2014 – Nov 2022, 15 features)
- Feature engineering: EMA, SMA, WMA, TEMA, DEMA, Bollinger Bands (7/30/90 day windows)
- Feature selection using Random Forest Regressor — top 10 features selected
- Trained and compared LSTM, SVR, and Linear Regression models
- Built real-time inference pipeline for next-day price prediction

## Tech Stack
Python · scikit-learn · TensorFlow/Keras · pandas-ta · BeautifulSoup · yfinance · pandas · numpy · pickle

## Model Results

| Model | Accuracy |
|---|---|
| LSTM | 76.8% |
| SVR | 84% |
| **Linear Regression (SGD)** ✅ | **90.56%** |

## Files
- `Prediction.ipynb` — model training notebook
- `inference.py` — real-time scrape + predict script
- `linear_reg_10_25.sav` — saved final model

## Published Paper
Bitcoin Investopedia — Chatbot, Market Predictor and Public Survey on Taxation  
Usha Horapeti et al. · PES University · IEEE
