# Time Series Analysis and Trading Strategy with ARIMA


## Project overview
This project demonstrates time series forecasting and quantitative trading strategies using Palantir Technologies Inc. (PLTR) stock data retrieved via yfinance. It includes:

✔️ Data preprocessing: Cleaning, splitting, and resampling time series data
✔️ Exploratory Data Analysis (EDA): Visualizing stock price trends, log returns, and distribution analysis
✔️ Seasonality and trend decomposition: Using statsmodels for additive/multiplicative decomposition
✔️ Autocorrelation & Partial Autocorrelation (ACF/PACF): Identifying optimal ARIMA parameters
✔️ ARIMA modeling: Time series forecasting using an ARIMA model
✔️ Trading strategy simulation: Implementing buy/sell signals based on forecasted values
✔️ Performance evaluation: Calculating Sharpe ratio, cumulative returns, and drawdown analysis

## Package used
* Python 🐍
* yfinance (Yahoo Finance API) 📊
* pandas (Data handling)
* numpy (Numerical computations)
* matplotlib / seaborn (Data visualization) 📈
* statsmodels (Time series modeling & ARIMA)
* scipy.stats (Statistical analysis)
* sklearn.metrics (Model evaluation)


## Implementation steps
1. Data Preprocessing
   * Downloading PLTR stock data using yfinance
   * Checking for missing values
   * Splitting data into training (90%) and testing (10%) sets
   * Resampling data into daily, monthly, quarterly intervals for better trend analysis
2. Exploratory Data Analysis (EDA)
   * Stock price visualization
   * Log returns & distribution analysis
   * Autocorrelation (ACF) & Partial Autocorrelation (PACF) plots for ARIMA tuning
   * Seasonal decomposition of trends
3. Time Series Forecasting with ARIMA
   * Using ARIMA for price prediction
   * Tuning parameters (p, q) based on AIC/BIC score
   * Rolling window forecast for more accurate predictions
   * Confidence intervals to assess prediction uncertainty
4. Trading Strategy
* Signal Generation:
   * Buy (1) if predicted price is higher than the current price
   * Sell (-1) if predicted price is lower than the current price
* Strategy Performance Evaluation:
   * Sharpe Ratio
   * Cumulative Returns
   * Drawdown Analysis

 ## Future Enhancements
* LSTM / Transformer models for deep learning-based forecasting
* Reinforcement Learning for adaptive trading strategies
* Multi-asset portfolio analysis with diversification metrics
