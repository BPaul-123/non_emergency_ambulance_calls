# Ambulance Demand Time Series Analysis  
  
## Overview  
This project applies time series modelling techniques to analyse monthly non-emergency ambulance call volumes. The aim is to identify trends, seasonal patterns, and build an appropriate forecasting model to understand service demand.  
  
---  
  
## Dataset  
The dataset consists of monthly non-emergency ambulance call volumes from 2013 to 2022.  
  
**Note:** The dataset is not included in this repository due to coursework restrictions.  
  
---  
  
## Methodology  
  
### Data Analysis  
- Time series visualisation  
- Trend and seasonality identification  
- Differencing to achieve stationarity  
  
### Modelling  
Several SARIMA models were evaluated to identify the best fit for the data.  
  
---  
  
## Model Selection  
  
The **SARIMA(2,1,1)(1,1,1)[12]** model demonstrated the best overall performance:  
  
- **AIC:** −781.20    
- **BIC:** −765.16    
- **AICc:** −780.36    
- **RMSE:** 0.00610    
- **MAE:** 0.00355    
  
These metrics indicate a strong model fit with minimal forecasting error.  
  
---  
  
## Model Diagnostics  
  
Residual diagnostics confirmed model adequacy:  
  
- Ljung–Box test (**p = 0.9585**) indicates no significant autocorrelation    
- Residual ACF and PACF plots show no remaining structure    
- Histogram and Q–Q plot suggest approximate normality of residuals    
  
---  
  
## Key Findings  
  
- A clear **upward trend** in ambulance call volumes over time    
- Strong **seasonal patterns**, likely reflecting recurring demand cycles    
- The selected SARIMA model effectively captures both trend and seasonality    
  
---  
  
## Conclusion  
  
The analysis of monthly non-emergency ambulance calls from 2013 to 2022 reveals a significant upward trend and pronounced seasonal variation. The SARIMA(2,1,1)(1,1,1)[12] model successfully captures these patterns, with diagnostic tests confirming that the model provides an adequate representation of the underlying data dynamics.  
  
---  
  
## Tools & Technologies  
- R  
- Time series analysis techniques  
- Forecasting models (SARIMA)  
- Data visualisation  
