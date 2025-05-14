# US PCE Forecasting - SARIMA and VAR
**Overview**:
As a major driver of economic growth, Private Consumption Expenditure (PCE) accounts for over 65% of the U.S. GDP. Given its significance, forecasting PCE is crucial for policymakers and analysts to understand economic trends.

**Objective**:
To develop and compare time series forecasting models that predict future trends in PCE with a high degree of accuracy.

**Dataset**:
The dataset is sourced from the Federal Reserve Economic Data (FRED), and comprises of the following variables <https://fred.stlouisfed.org/categories>:
1. PCE (monthly in billions of USD)
2. Disposable Personal Income (billions of dollars)
3. Price Index (PCE-based)
4. Total Federal Outlay (billions of USD)
   
**Methodology**:
1. SARIMA (Seasonal AutoRegressive Integrated Moving Average):
   A univariate time series model used to forecast PCE based on its own past values and seasonality patterns.
3. VAR (Vector AutoRegression):
   Multivariate time series model that captures the interdependencies between PCE and related macroeconomic indicators.

**Findings**:
Incorporating multiple economic indicators using VAR significantly enhanced forecast accuracy. Compared to the SARIMA model, the VAR model increased the R-squared value from 0.86 to 0.96, a 10-percentage-point increase, thereby highlighting the benefits of accounting for macroeconomic interdependencies in forecasting. It is important to note that the model was revised to train the model on data from 1st January 2022, instead of 1st January 1980 -- the COVID-19 pandemic brought in systemic changes, thereby making the previous data meddle with the trend from 2022-onwards.
