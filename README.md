# AR(1) Time Series Forecasting with Python

This project demonstrates a simple yet powerful approach to forecasting monthly revenue using an Autoregressive (AR) model in Python. Leveraging the `statsmodels` library, we:

1. **Load & Clean Data**  
   – Prepare a time-indexed pandas DataFrame from CSV/Google Sheets export.  
2. **Stationarity Test**  
   – Run the Augmented Dickey–Fuller test to confirm data is already stationary (d=0).  
3. **Model Selection**  
   – Compare SARIMA(1,0,0)(0,0,1,12) vs. AR(1) (i.e. SARIMA(1,0,0)(0,0,0,12)), evaluating AIC, residual diagnostics, and Ljung–Box tests.  
4. **Fit AR(1) Model**  
   – Finalize on AR(1) based on parsimony and diagnostic results.  
5. **1-Month Ahead Forecast**  
   – Generate point forecast and 95% confidence interval for the next period.  
6. **Visualization**  
   – Plot historical series and forecast with shaded confidence bands.

🔗 **Colab Notebook:** [arima_model.ipynb](https://colab.research.google.com/drive/1POdhvK-LRMdlmVv-TcStCWaxi7I8WgUI?usp=sharing)

## Key Highlights
- **Minimal Dependencies:** Python 3, pandas, matplotlib, statsmodels  
- **Transparent Diagnostics:** ADF test, ACF/PACF analysis, residual checks  
- **Reproducible Workflow:** From data prep to forecasting in a single notebook  

Feel free to fork, explore alternative parameter grids, or adapt for your own time series forecasting needs!  

---
