# Forecast Direct Normal Irradiance of Solar Energy

This project aims to forecast short-term and long-term Direct Normal Irradiance, which is crucial in solar energy. Nowadays, the adoption of solar energy into the power grid has increased, and it has become essential to accurate forecasts of direct normal irradiance from solar power for the effective operation and maintenance of power systems, ensuring their ability. Photovoltaic panels track the sun to receive more DNI. DNI accounts for a large portion of PV solar energy.

## Authors
- [Md Mehedi Hasan](https://github.com/mmh52)
- [Kamlesh Sarkar](https://github.com/ksarkar420)

## Project Overview

- **Dataset:** In this project, we use a dataset from Lowery Power Station, Denver, Colorado, covering the period from June 2008 to December 2013. This dataset contains Direct Normal irradiance, Globa Horizontal, and other features of Solar Energy. 

- **Preprocess Data:** This dataset contains minute data of direct normal irradiance and has some anomalies. We fixed those anomalies, filled in missing values, and converted it to an hourly dataset.

- **Key performance indicator:** We used RMSE (Root Mean Square Error) metrics to measure the performance of all models based on short-term and long-term forecasting of DNI.

- **Stakeholders:** Accurate DNI predictions help Operation and Maintenance (O&M) Service Providers in optimizing solar panel orientation for CSP systems and schedule maintenance during low DNI periods to minimize disruption. Also, forecasting DNI aids grid operators in managing solar power integration, balancing supply and demand, maintaining grid stability, and reducing fossil fuel reliance. These predictions are also crucial for assessing the financial viability of solar projects, enabling investors to estimate returns and make informed funding decisions.

- **Models:** To forecast Direct Normal Irradiance, we used time series forecasting models

     - **Tripple Exponential Smoothing:** The univariate exponential smoothing model uses the rolling average technique, in which the weights of previous time stamps 
       decrease exponentially. In this project, we used an additive version of triple exponential smoothing that can capture the seasonality of time series. 
     
     - **ARIMA:** ARIMA is another univariate time series Model that combines autoregressive (AR) terms, differencing (I), and moving average (MA) terms. This 
       model is suitable for data that can be made stationary through differencing. 
     
     - **SARIMA:** SARIMA is an extended version of ARIMA that can capture seasonal components of time series data. The dataset in our project represents seasonality, so 
        SARIMA is a suitable model for our project. 
     
     - **SARIMAX:**  SARIMAX extends SARIMA by including exogenous variables in the model. This model is suitable if other features of the time series data play an important 
       role in forecasting feature values. In our project, we pick the Zenith Angle as an exogenous variable to forecast direct normal irradiance.


## Future Work 

- Incorporate weather and cloud cover data, which can be important features for forecasting direct normal irradiance.
- Use multivariate deep learning models that can incorporate all important features of solar energy and forecast direct normal irradiance more accurately.


## Sources
[1] Lowery Power Station Dataset: http://dx.doi.org/10.5439/1052550

[2] Hosseini, M.; Katragadda, S.; Wojtkiewicz, J.; Gottumukkala, R.; Maida, A.; Chambers, T.L. Direct Normal Irradiance Forecasting Using Multivariate Gated Recurrent Units. Energies 2020, 13, 3914. https://doi.org/10.3390/en13153914

[3] E. Cogliani. The role of the direct normal irradiance (DNI) forecasting in the operation of solar concentrating plants. https://doi.org/10.1016/j.egypro.2014.03.170
