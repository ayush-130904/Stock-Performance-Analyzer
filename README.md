## Stock Performance Analyzer 📈
A Python-based financial analysis tool that fetches real-time market data to evaluate stock performance. This project calculates key technical indicators like Moving Averages and Volatility to provide trend analysis and price range predictions.

## 🚀 Features
Real-time Data: Integration with yfinance to fetch the latest stock prices.
Technical Indicators: Calculates the 20-day Moving Average (MA20) to identify market trends.
Risk Assessment: Computes daily volatility (Standard Deviation) to quantify stock risk.
Predictive Analysis: Generates a predicted high/low price range for the next trading day based on current volatility.
Automated Trend Logic: Provides an instant "Bullish" or "Bearish" signal based on price position relative to the moving average.

## 🛠️ Tech StackPython 
3.xPandas: For data manipulation and time-series analysis.
NumPy: For mathematical calculations and volatility modeling.
yfinance: To download historical market data from Yahoo Finance.

## 📦 InstallationClone the repository:
```
git clone https://github.com/ayush-130904/Stock-Performance-Analyzer.git
```
```
cd Stock-Performance-Analyzer
```

Install required dependencies:
```
pip install pandas numpy yfinance
```

### 🖥️ UsageOpen the stock_performance_analyzer.ipynb in Jupyter Notebook, VS Code, or Google Colab.
Run the cells sequentially.When prompted, enter a stock ticker symbol (e.g., AAPL for Apple, RELIANCE.NS for Reliance, or ^NSEI for Nifty 50).View the analysis summary and trend advice.

### 📊 Sample OutputPlaintext
```
Enter Stock Name/Symbol: ^NSEI
---Fetching data from ^NSEI---

Stock Name : NIFTY 50
Current Price : 26178.70rs
20 Day Moving Average : 26023.98rs
Daily Risk : 0.44%
Predicted Range for tomorrow: 26063.22rs to 26294.18rs


TREND: The stock is currently above its 20-day average (Bullish).
```

## 🧠 Logic Breakdown
Volatility Calculation: The program calculates the percentage change of daily closing prices and determines the standard deviation to represent "Daily Risk."\n
Moving Average: Uses a rolling 20-day window to smooth out price fluctuations and identify the medium-term trend.\n
Prediction: The predicted range is calculated as:$Upper Bound = Last Price \times (1 + Volatility\%)$$Lower Bound = Last Price \times (1 - Volatility\%)$

