# Microsoft (MSFT) Stock Price Prediction Using LSTM

A deep learning time-series forecasting project that uses a Long Short-Term Memory (LSTM) neural network to predict Microsoft (MSFT) stock closing prices using historical market data.

The project covers the complete machine learning workflow, from historical data preparation and exploratory analysis to LSTM training, model evaluation, recursive forecasting, and future price prediction.

---

## 📌 Project Overview

Stock prices form a time series where historical observations can provide useful information about future price movements. However, financial markets are highly complex and influenced by numerous factors such as economic conditions, company performance, market sentiment, geopolitical events, and unexpected news.

This project explores whether an **LSTM neural network** can learn patterns from historical Microsoft stock prices and use those patterns to predict future closing prices.

The model uses the previous **3 trading days of MSFT closing prices** to predict the next closing price.

The project also compares the LSTM against a simple **naive baseline**, where the next day's price is predicted to be equal to the current day's price.

The goal is not to build a guaranteed stock-picking system, but to investigate the effectiveness of LSTM-based time-series forecasting on historical MSFT stock data.

---

## 🎯 Objectives

The main objectives of this project are:

- Analyze historical Microsoft stock price data.
- Perform data cleaning and validation.
- Explore long-term MSFT price trends.
- Analyze daily returns and moving averages.
- Convert the time-series data into supervised learning windows.
- Split the data into training, validation, and testing datasets.
- Establish a naive forecasting baseline.
- Build an LSTM neural network for stock-price prediction.
- Train the model using validation data and early stopping.
- Evaluate predictions using multiple regression metrics.
- Measure directional prediction accuracy.
- Analyze prediction errors.
- Perform recursive forecasting.
- Generate a 30-trading-day future forecast.
- Compare the LSTM model against a naive baseline.

---

## 📊 Dataset

The project uses historical Microsoft Corporation (`MSFT`) stock market data.

### Data Source

The dataset contains historical daily market information for Microsoft stock.

### Date Range

**March 13, 1986 – August 3, 2026**

### Original Columns

The dataset contains:

| Column | Description |
|---|---|
| `Date` | Trading date |
| `Open` | Opening price |
| `High` | Highest price during the trading day |
| `Low` | Lowest price during the trading day |
| `Close` | Closing price |
| `Adj Close` | Adjusted closing price |
| `Volume` | Number of shares traded |

For the initial LSTM experiment, the model focuses on the **Close** price.

---

## 🧠 Why LSTM?

Traditional neural networks do not naturally handle sequential dependencies.

LSTM networks are a type of recurrent neural network designed to learn patterns across sequences.

For stock-price forecasting, an LSTM can use a sequence such as:

Day 1 Close
Day 2 Close
Day 3 Close
     ↓
Predicted Day 4 Close
This project uses a Long Short-Term Memory (LSTM) neural network
to predict Microsoft (MSFT) stock closing prices.

The project covers:

- Historical stock price analysis
- Data cleaning and validation
- Exploratory data analysis
- Moving averages
- Time-series window generation
- Train/validation/test splitting
- Naive baseline forecasting
- LSTM model training
- Training and validation loss analysis
- Model evaluation
- Directional accuracy
- Prediction error analysis
- Recursive forecasting
- 30-trading-day future forecasting


# Conclusion

This project developed an LSTM-based time-series forecasting model
for Microsoft (MSFT) stock closing prices.

The workflow included:

1. Historical MSFT stock data preparation
2. Data quality validation
3. Exploratory data analysis
4. Moving-average analysis
5. Time-series window generation
6. Train/validation/test splitting
7. Naive baseline forecasting
8. LSTM model training
9. Early stopping
10. Model evaluation using MAE, RMSE, MAPE and R²
11. Directional accuracy analysis
12. Prediction-error analysis
13. Recursive forecasting
14. 30-trading-day future forecasting

The LSTM model should be evaluated against the naive baseline rather
than judged only from the prediction graph.

The results should be interpreted carefully because stock prices are
affected by many external factors that are not included in this
close-price-only model.

## Limitations

- The current model uses only historical closing prices.
- It does not include market news or macroeconomic variables.
- It does not account for sudden market events.
- Recursive forecasts can accumulate prediction errors.
- Historical performance does not guarantee future performance.

Therefore, this project is intended as a machine-learning
time-series forecasting experiment and not as financial advice.

# Future Improvements

The next version of this project can be improved by introducing
additional features and models.

## Possible improvements

### Feature Engineering

Add:

- Open
- High
- Low
- Volume
- Daily returns
- RSI
- MACD
- Bollinger Bands
- Moving averages
- Volatility

### Model Improvements

Compare:

- Naive baseline
- Linear Regression
- Random Forest
- XGBoost
- Basic LSTM
- Stacked LSTM
- GRU
- Bidirectional LSTM

### Advanced Experiments

- Hyperparameter tuning
- Different lookback windows
- Multi-feature LSTM
- Attention mechanisms
- Transformer-based time-series models

The goal of future experiments would be to determine whether
additional features or more complex architectures can consistently
outperform the baseline model on unseen data.
