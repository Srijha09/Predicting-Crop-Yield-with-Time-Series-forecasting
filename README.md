## Predicting-Crop-Yield-with-Time-Series-forecasting

This project focuses on predicting crop yield using historical environmental data and time series forecasting techniques. By analyzing key factors such as daily precipitation, soil moisture, temperature, and vegetation indices, we can forecast future production quantities with improved accuracy. This can aid farmers and agricultural stakeholders in optimizing resources and planning for future crop cycles.

Overview
Agricultural yield prediction is essential for optimizing the allocation of resources, minimizing waste, and ensuring food security. In this project, we utilize time series forecasting techniques to predict crop yields based on a combination of historical data, environmental variables, and vegetation health indicators.

The project leverages various datasets, including daily precipitation, soil moisture, temperature, and the Normalized Difference Vegetation Index (NDVI), to make informed predictions about future crop yields.

### Dataset
The following datasets are used in this project:

Daily Precipitation.csv: Contains daily records of precipitation levels, which are vital for understanding crop water availability.

Daily Soil Moisture.csv: Daily soil moisture levels, indicating the water retention in the soil over time.

Daily Temperature.csv: Captures temperature data over time, a key factor affecting crop growth.

Eight Day NDVI.csv: Normalized Difference Vegetation Index (NDVI) over eight-day intervals to measure the health and greenness of the vegetation.

Production Quantity.csv: Historical crop production quantities (target variable) used for model training.

predicted_production_qty.csv: The model’s predicted future crop yield based on historical patterns.

### Methodology
Data Preprocessing:
Handled missing data and performed data cleaning to ensure consistency.
Aggregated daily data into meaningful time intervals (e.g., weekly or monthly averages).
Normalized and scaled input data for better model performance.

### Feature Engineering:
Generated lagged features to account for temporal dependencies in the data.
Included external factors (precipitation, soil moisture, temperature, NDVI) as predictors to enhance model accuracy.

### Modeling(Multivariate time series analysis):

We implemented the following models:

ARIMA/SARIMA: Traditional time series forecasting methods that capture trends and seasonality in crop yields.

LSTM (Long Short-Term Memory): A deep learning model capable of learning complex temporal dependencies from sequential data.

Other potential models, such as Prophet, were considered for handling irregular time series data.
