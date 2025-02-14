# Tesla Stock Data Time Series Analysis

## Introduction
This project analyzes Tesla's stock data up to 2025 using time series methods. Our goal is to explore historical trends, daily changes, and internal correlations without making future predictions.

## Dataset
The dataset contains daily stock information for Tesla, including:
- **Date:** The trading day.
- **Open:** The price at the start of the day.
- **High:** The highest price during the day.
- **Low:** The lowest price during the day.
- **Close:** The price at the end of the day.
- **Adj Close:** The adjusted closing price (accounting for splits/dividends).
- **Volume:** The number of shares traded.

## Analysis Steps

### 1. Data Loading and Preparation
- **Download and Import Data:**  
  We used the KaggleHub API to download the latest Tesla stock data.
- **Data Loading:**  
  The data was loaded into a Pandas DataFrame.
- **Date Conversion:**  
  The 'Date' column was converted from text to datetime format and set as the DataFrame index. This allows for easy time-based operations and visualizations.

### 2. Exploratory Data Analysis (EDA)
- **Basic Inspection:**  
  We checked the shape, data types, and basic statistics of the dataset.
- **Trend Visualization:**  
  The closing price was plotted over time to observe overall trends.

### 3. Daily Returns and Volatility
- **Daily Returns:**  
  We calculated the percentage change in the closing price from one day to the next. This shows how much the stock changes daily.
- **Volatility Analysis:**  
  A histogram of daily returns was created to visualize the distribution and understand how volatile Tesla's stock is.

### 4. Moving Averages
- **Smoothing Data:**  
  Moving averages (e.g., 50-day and 200-day) were computed to smooth out short-term fluctuations and reveal longer-term trends.
- **Visualization:**  
  The moving averages were plotted alongside the closing price for better insight into trends.

### 5. Time Series Decomposition
- **Decomposition:**  
  We used seasonal decomposition to break the closing price into three components:
  - **Trend:** The long-term movement.
  - **Seasonal:** Repeating patterns or cycles.
  - **Residual:** Random noise.
- **Purpose:**  
  This step helps understand underlying patterns in the stock price data.

### 6. Autocorrelation Analysis
- **ACF and PACF:**  
  We analyzed the autocorrelation (ACF) and partial autocorrelation (PACF) of daily returns.
- **Goal:**  
  These plots show how past values relate to current values and if there are any repeating patterns (lags) in the data.

## Tools and Libraries
- **Pandas:** For data manipulation and analysis.
- **Matplotlib & Seaborn:** For creating visualizations.
- **Statsmodels:** For time series decomposition and autocorrelation analysis.
- **KaggleHub:** For downloading the dataset.

## Conclusion
This project provides a detailed time series analysis of Tesla's stock data. By exploring trends, daily changes, and autocorrelations, we gain a clear understanding of the historical behavior of Tesla stock. This analysis forms a solid foundation for further studies in financial data analysis, though no predictions are made in this project.

## Next Steps
Future work could include:
- Further exploring seasonal patterns in the data.
- Comparing Tesla's trends with market indices or other stocks.
- Delving deeper into volatility and other risk metrics.

Enjoy your exploration into time series analysis with this Tesla stock data project!

