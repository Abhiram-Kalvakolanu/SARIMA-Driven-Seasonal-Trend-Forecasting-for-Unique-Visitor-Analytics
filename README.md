<img src="https://github.com/user-attachments/assets/d10a9355-7fab-4aed-b9c7-37dacbafd66b" alt="Image" width="400"/>

# SARIMA-Driven Seasonal Trend Forecasting for Unique Visitor Analytics

## Project Description
This project focuses on analyzing and predicting the number of **unique visits** to an online shop using **time series data**. The dataset includes features such as `Day`, `Day.Of.Week`, `Date`, `Page.Loads`, `Unique.Visits`, `First.Time.Visits`, and `Returning.Visits`, with `Unique.Visits` as the target variable.

### Key Steps
1. **Data Preprocessing**  
   - Unified inconsistent date formats into a `datetime` structure.  
   - Sorted the dataset by `Date` for time series consistency.  
   - Verified no missing values and displayed basic statistical metrics.  

2. **Stationarity Analysis**  
   - Performed the **Augmented Dickey-Fuller (ADF) Test** to assess stationarity.  
   - Applied **first-order differencing**, confirming stationarity through plots and statistical tests.  

3. **Time Series Decomposition**  
   Decomposed the data into:
     - **Original Series**  
     - **Trend**  
     - **Seasonality**  
     - **Residuals**  

4. **Modeling Approach**  
   - Built a **Seasonal Autoregressive Integrated Moving Average (SARIMA)** model.  
   - Determined seasonal and autoregressive components using **ACF** and **PACF** plots.  

5. **Model Validation**  
   - Conducted residual analysis to ensure minimal autocorrelation.  
   - Validated assumptions through:
     - Residual histograms and Q-Q plots.  
     - Correlograms confirming independence of errors.  

6. **Forecasting**  
   - Predicted `Unique.Visits` for the next **100 days**, capturing seasonal trends consistent with historical data.

 
## Conclusion
The SARIMA model successfully captured **seasonality**, **trends**, and **residuals** of the time series. Residual diagnostics confirmed the model's reliability, with errors following a normal distribution. This project demonstrates the effective use of SARIMA for analyzing and forecasting time series data with strong seasonal components. It provides a robust framework for tackling similar predictive analytics problems.

