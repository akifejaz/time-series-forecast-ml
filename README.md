# time-series-forecast-ml
A Python project for forecasting future values in a time series using machine learning models.

## Overview
This project aims to provide a simple and easy-to-use tool for forecasting future values in a time series using machine learning techniques. The project includes several popular models for time series forecasting such as ARIMA, SARIMA, and LSTM. The user can easily train and evaluate the models using their own time series data.

## Installation
To install the package, use the following command:
```
pip install time-series-forecasting

```

## Usage
The package includes the following main functions:

1. fit(model, data): trains a specified model on the provided time series data.
2. predict(model, data, steps): makes predictions for the next steps steps in the time series using a trained model.
3. evaluate(model, data): evaluates the performance of a trained model on the provided time series data. The package also includes sample datasets that can be used for testing and demonstration.


```
from time_series_forecasting import *
# load data
data = load_data("sample_data")
# train the model
model = fit(SARIMA, data)
# make predictions
predictions = predict(model, data, steps=10)
# evaluate the model
evaluate(model, data)

```

## Models
The package currently includes the following models for time series forecasting:

1. ARIMA: Autoregressive Integrated Moving Average model
2. SARIMA: Seasonal Autoregressive Integrated Moving Average model
3. LSTM: Long Short-Term Memory model

## Requirements
The package requires the following libraries:

1. numpy
2. pandas
3. scikit-learn
4. statsmodels
5. keras

## Contributing
We welcome contributions to this project. If you are interested in contributing, please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for more information.

## References
Forecasting: Principles and Practice by Rob J Hyndman and George Athanasopoulos
Deep Learning for Time Series Forecasting by Jason Brownlee
