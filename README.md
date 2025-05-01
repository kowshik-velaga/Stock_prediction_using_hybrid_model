# 📈 Stock Price Prediction using Hybrid TCN + Transformer Model

This project demonstrates a deep learning approach for next-day stock price prediction using a hybrid architecture that combines **Temporal Convolutional Networks (TCNs)** and **Linformer-based Transformer attention**. The model is trained on historical OHLCV data enriched with technical indicators such as RSI, SMA, and Bollinger Bands.

---

## 🧠 Objective
To build a robust time-series forecasting model that learns sequential patterns in stock data and provides accurate next-day closing price predictions.

---

## 🔍 Overview

### ✅ Technologies Used
- Python  
- TensorFlow / Keras  
- TA-Lib (Technical Analysis Library)  
- yFinance API  
- Linformer (efficient attention)  
- Matplotlib & Seaborn (for visualization)

---

### 🔧 Pipeline

1. **Data Collection**  
   - Historical stock data fetched using `yfinance`  
   - Stocks like AAPL, MSFT, etc., over a configurable date range

2. **Feature Engineering**  
   - Technical indicators:  
     - SMA (Simple Moving Average)  
     - RSI (Relative Strength Index)  
     - Bollinger Bands  
   - Features are normalized and converted into sequences

3. **Model Architecture**
   - **TCN Block**: Causal 1D convolutions with dilation to capture temporal dependencies  
   - **Linformer**: Efficient self-attention for long-range dependencies  
   - **Dense Layers**: For final regression output

4. **Training & Evaluation**  
   - Split into Train, Validation, and Test sets  
   - Loss: MSE (Mean Squared Error)  
   - Metrics: MAE (Mean Absolute Error)  
   - Visualization: Actual vs Predicted close prices

---

## 🏆 Results
- Achieved low MSE and MAE on the test set
- Predicted close prices closely follow actual market behavior
- Hybrid model captures both short-term patterns and long-term dependencies

---

## 📊 Visual Output

<img src="https://your-image-link.com/actual-vs-predicted.png" alt="Prediction Chart" width="600"/>

---

## 🚀 Future Enhancements
- Add hyperparameter tuning using Optuna or Keras Tuner  
- Deploy model as a REST API or Streamlit dashboard  
- Extend to multi-day or multi-stock forecasting  
- Incorporate sentiment analysis and macroeconomic indicators

---

## 👤 Author
**Krishna Kowshik**  
📫 [LinkedIn]((https://www.linkedin.com/in/sai-krishna-kowshik-velaga-2942a4252/)) | 📧 krishnakowshik312@gmail.com  

---

## 📁 Files
- `stock-prediction-using-hybrid-tcn.ipynb`: Main notebook with all code and visualizations  
- `README.md`: Project overview (this file)

---

## 📝 License
This project is open for academic and non-commercial use. Contact for collaboration or licensing inquiries.
