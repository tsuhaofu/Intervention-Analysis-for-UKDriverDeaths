# Intervention Analysis of UKDriverDeaths Dataset

This project investigates the effect of the seatbelt law implementation on the number of car drivers killed or seriously injured in the UK, utilizing a time-series analysis approach with intervention analysis.

## Introduction
This analysis uses the UKDriverDeaths dataset, covering data from January 1969 through December 1984, known as the "seatbelt data". This dataset was pivotal in evaluating the effectiveness of the compulsory seatbelt legislation introduced on January 31, 1983. The aim is to assess the impact of this intervention on reducing fatalities.

## Data
The dataset consists of monthly counts of car drivers killed or seriously injured in the UK. It shows clear trends and seasonality, which were addressed to achieve stationarity and improve forecasting accuracy.

## Exploratory Data Analysis (EDA)
- **Trend Analysis**: The data exhibit a long-term decrease in driver deaths, potentially influenced by various factors, including improvements in road safety and vehicle technology.
- **Seasonality**: Regular fluctuations are evident, likely related to seasonal variations in driving conditions, such as winter weather.
- **Intervention Point**: The introduction of the seatbelt law is marked, showing a noticeable decrease in fatalities, indicating the law's potential effectiveness.
- **Log Transformation**: Applied to stabilize variance and improve the normality of the data distribution.

## Methodology
### Statistical Testing
- **Stationarity Tests**: Both Augmented Dickey-Fuller (ADF) and KPSS tests were conducted to confirm the trend stationarity of the data, requiring differencing to achieve stationarity.
### Pre-Intervention Modeling
- **SARIMA Model**: Employed for modeling and forecasting. SARIMA(0, 1, 1)(0, 1, 1)[12], known as the airline model, included both non-seasonal and seasonal components. Specific parameters were chosen based on the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) analyses.

### Intervention Analysis
- **Introduction of Intervention Variable**: The implementation of the seatbelt law marked by the intervention variable in the SARIMA model showed a significant reduction in the number of deaths, confirming the law's effectiveness.
- **T-tests**: Conducted to compare the means before and after the law implementation, showing statistically significant differences.

### Forecasting 
Forecasting using the model showed a clear divergence in expected fatalities with and without the seatbelt legislation, underscoring the law's beneficial impact.

## Results
- **Model Fit**: The SARIMA(0, 1, 1)(0, 1, 1)[12] model fits well, capturing seasonal spikes and trends effectively.
- **Intervention Impact**: The intervention coefficient of -0.2278 with a very low p-value suggests a significant decrease in fatalities due to the seatbelt law.

## Conclusion
The study successfully demonstrates the seatbelt law's effectiveness using time-series analysis. The SARIMA model, complemented by intervention analysis, provides strong evidence of the law's positive impact on road safety.


