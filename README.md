# Electricity Consumption Time-Series Analysis and Forecast

- **The detailed report can be found  [here](https://github.com/CarlosTussi/electricity-timeseries/blob/main/report.pdf)**

- The goal of this project is to find the best model to forecast the energy consumption during a 15 minutes
interval on a single day (21/02/2010). In order to do that, EDA is done to analyze the data set and clean
it when needed. After, Feature Engineering is performed to try to get a better insight and find underlying
information in the data (such as days of the week’s influence and different daily consumption demand levels),
including possible outliers.

- In the modeling part, different types of models are tested with different hyper parameters (both statistical
and machine learning models). The models are trained both with the covariate temperature and without it,
in order to analyze its impact in the overall result. The models are compared using the MSE metric.

- For the best model, cross-validation is performed with different splits of the train and test set to confirm
that no overfitting is present. Finally, the models are retrained with the whole dataset to obtain the final
best model: best model without temperature covariate and best model with the temperature covariate.
