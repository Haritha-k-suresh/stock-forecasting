TIME SERIES ANALYSIS AND FORECASTING FOR STOCK MARKET 
# 📈 Stock Market Analysis & Forecasting

This project explores various time series forecasting techniques to predict stock prices using **AAPL (Apple Inc.) stock data from Yahoo Finance**. The analysis spans from classical statistical models like ARIMA and SARIMA to deep learning approaches including LSTM and Bidirectional LSTM.

---

## 🧠 Models Implemented

### 1. 🔹 ARIMA (AutoRegressive Integrated Moving Average)
- Captures linear trends using autoregressive and moving average components.
- Assumes the data is stationary (differencing applied if necessary).
- **Performance**: Good for stable patterns but fails to capture sudden volatility.

### 2. 🔺 SARIMA (Seasonal ARIMA)
- Extension of ARIMA that incorporates **seasonality**.
- Suitable for data with regular periodic trends.
- **Performance**: Slightly better than ARIMA on seasonal behavior but still underperforms in capturing non-linear fluctuations.

### 3. 📅 Prophet
- Developed by Facebook, Prophet is robust to missing data and handles holidays, trends, and seasonality well.
- Automatically handles trend changepoints.
- **Performance**: Highly interpretable; performs decently, but struggles with short-term volatility.

### 4. 🔮 LSTM (Long Short-Term Memory)
- Deep learning model specialized for sequential data.
- Captures non-linear relationships and long-term dependencies.
- **Performance**: Significantly better at modeling volatile, noisy stock prices compared to classical models.

### 5. 🔁 Bidirectional LSTM (BiLSTM)
- An extension of LSTM that learns patterns from **past and future contexts** simultaneously.
- Tuned with:
  - Increased number of LSTM units
  - Dropout for regularization
  - Optimized sequence length and batch size
- **Performance**:
  - Outperforms all other models on MAE and RMSE.
  - Captures both trend and volatility more effectively.
  - Provides more accurate short- and mid-term forecasts.

---

## 🧪 Evaluation Metrics

| Model         | MAE    | RMSE   |
|---------------|--------|--------|
| ARIMA         | 2.41   | 2.87   |
| SARIMA        | 2.71   | 3.07   |
| Prophet       | 16.86  | 17.19  |
| LSTM          | 4.81   | 5.90   |
| Bi-LSTM       | 2.88   | 3.65   |


## 📃 License

MIT License


