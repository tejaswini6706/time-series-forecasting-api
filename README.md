# 📊 End-to-End Time Series Forecasting System with API

## 🚀 Overview
This project builds a production-ready time series forecasting system to predict sales for the next 8 weeks for each state using historical data.

The system includes:
- Data preprocessing  
- Feature engineering  
- Multiple model training  
- Model comparison  
- Automatic best model selection  
- REST API for predictions  

---

## 🎯 Objective
- Forecast sales for the next 8 weeks  
- Handle missing values and missing dates  
- Capture trend and seasonality  
- Compare multiple models  
- Serve predictions using API  

---

## 📂 Dataset
- Format: Excel  
- Columns: Date, State, Sales  

### Preprocessing:
- Converted date column to datetime  
- Sorted data by date  
- Handled missing dates using resampling  
- Filled missing values  

---

## 🛠️ Feature Engineering
- Lag Features: t-1, t-7, t-30  
- Rolling Mean & Standard Deviation  
- Day of Week, Month  
- Holiday Feature (if applicable)  

---

## 🤖 Models Used
- SARIMAX (ARIMA / SARIMA)  
- Prophet  
- XGBoost  
- LSTM  

---

## 📈 Model Evaluation
- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  

Best model selected based on lowest error.

---

## 🔮 Forecast Output
- Predicts next 8 weeks  
- State-wise predictions  

Example:
```json
{
  "state": "XYZ",
  "forecast": [
    {"date": "2026-01-01", "sales": 1200}
  ]
}
