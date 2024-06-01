# Forecast Direct Normal Irradiance of Solar Energy

This project aims to forecast a week ahead solar energy via Direct Normal Irradiance. Nowadays, the adoption of solar energy into the power grid has increased, and it has become essential to accurate forecasts of direct normal irradiance from solar power for the effective operation and maintenance of power systems, ensuring their ability. Photovoltaic panels track the sun to receive more DNI. DNI accounts for a large portion of PV solar energy. Forecasting DNI for the long term is a very cumbersome task.


## Project Overview

- ** Dataset:** In this project, we use a dataset from Lowery Power Station covering the period June 2008 to December 2013. This dataset contains Direct Normal irradiance, Globa Horizontal, and other features of Solar Energy. 

- ** Preprocess Data:** This dataset contains minute data of direct normal irradiance and has some anomalies. We fixed those anomalies, filled in missing values, and converted it to an hourly dataset.

- ** Models:** To forecast Direct Normal Irradiance, we used time series forecasting models

     - Exponential Smoothing
     
     - ARIMA
     
     - SARIMA
     
     - SARIMAX



## Sources
[1] Lowery Power Station Dataset: http://dx.doi.org/10.5439/1052550

[2] Hosseini, M.; Katragadda, S.; Wojtkiewicz, J.; Gottumukkala, R.; Maida, A.; Chambers, T.L. Direct Normal Irradiance Forecasting Using Multivariate Gated Recurrent Units. Energies 2020, 13, 3914. https://doi.org/10.3390/en13153914

[3] E. Cogliani. The role of the direct normal irradiance (DNI) forecasting in the operation of solar concentrating plants. https://doi.org/10.1016/j.egypro.2014.03.170
