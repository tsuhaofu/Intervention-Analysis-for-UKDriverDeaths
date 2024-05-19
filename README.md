# Intervention Analysis for UKDriverDeaths Dataset

This project investigates the effect of the seatbelt law implementation on the number of car drivers killed or seriously injured in the UK, utilizing a time-series analysis approach with intervention analysis.

## Introduction
This analysis uses the UKDriverDeaths dataset, covering data from January 1969 through December 1984, known as the "seatbelt data". This dataset was pivotal in evaluating the effectiveness of the compulsory seatbelt legislation introduced on January 31, 1983. The aim is to assess the impact of this intervention on reducing fatalities.

## Data
The dataset consists of monthly counts of car drivers killed or seriously injured in the UK. It shows clear trends and seasonality, which were addressed to achieve stationarity and improve forecasting accuracy.

## Exploratory Data Analysis (EDA)
- **Trend Analysis**: The data exhibit a long-term decrease in driver deaths, potentially influenced by various factors, including improvements in road safety and vehicle technology.
- **Seasonality**: Regular fluctuations are evident, likely related to seasonal variations in driving conditions, such as winter weather.

## Methodology
### Data Transformation
- **Log Transformation**: Applied to stabilize variance and improve the normality of the data distribution.
- **Differencing**: Used to remove trends and seasonality, achieving stationarity necessary for the subsequent time-series analysis.

### Time-Series Decomposition
- **Additive Decomposition**: Applied to separate the time series into trend, seasonal, and random components, facilitating a clearer understanding of underlying patterns.

### Model Building
- **SARIMA Model**: Employed for modeling and forecasting. The model, known as the airline model, included both non-seasonal and seasonal components. Specific parameters were chosen based on the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) analyses.

## Intervention Analysis
- **Impact of Seatbelt Law**: The implementation of the seatbelt law marked by the intervention variable in the SARIMA model showed a significant reduction in the number of deaths, confirming the law's effectiveness.

## Statistical Testing
- **Stationarity Tests**: Both Augmented Dickey-Fuller (ADF) and KPSS tests were conducted to confirm the stationarity of the data.
- **T-tests**: Conducted to compare the means before and after the law implementation, showing statistically significant differences.

## Results
- **Model Fit**: The SARIMA model fit the data well, capturing the autocorrelations and seasonality effectively.
- **Forecasting**: Forecasts made from the model indicate a continued effect of the seatbelt law on reducing fatalities, diverging from what might have been expected without the intervention.

## Conclusion
The analysis demonstrates the significant impact of seatbelt legislation on reducing fatalities in the UK. The intervention analysis, backed by robust statistical testing and time-series modeling, provides compelling evidence of the law's effectiveness.


