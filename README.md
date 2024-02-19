# CE888 A
CODE RUN: The ipynb file at first needs to be uploaded in Google colab or jupyter notebook along with the dataset.
Once it is uploaded there is one menu bar named runtime in the google colab and in there click on Run All if someone wants to run the whole ipynb file at oce

Brighton Dataset:
The dataset at first is read using the pandas dataframe. The dataset contains lots of missing values and imputation techniques is used in order to fill the missing column as it is essential before building any model and doing prediction. Missing values in these columns 'temp', 'dew', 'humidity', 'windspeed', 'winddir','sealevelpressure', 'cloudcover', 'solarradiation','solarenergy', 'uvindex' are filled with their mean values. Some other columns like 'precip', 'snowdepth', 'precipprob', 'preciptype','snow' where missing value is present is filled with 0. Data and time column is converted into proper format and then some of the data visualization is done with the help of matplotlib and seaborn libraries.After that splitting of data is done and features importance is selected

Colchester Dataset:
Once the dataset is imported it is seen that there are many missing values in the data.. So median imputation is used in order to fill the missing in all columns except preciptype column which contains more than 90% missing value and so it is dropped. Then some of the preprocessing and EDA is done on this dataset.

#### My main goal for the next assignment is to build some deep learning and time series analysis model and comapre the performance and determine which model is preforming better by taking evaluation metrics like MSE,MAPE and RMSE. The model which will have lower value means the performance is better. Finally future forecasting for next couple of days will be done for columns like humidity and temperature


#### ASSUMPTIONS FOR COLCHESTER DATASET
Many inferences may be drawn from the dataset provided:
(a)Uniform Sampling Interval: Assuming a constant temporal frequency, the data seems to be sampled at regular intervals (such as hourly).
(b)Data quality: The dataset could include missing values (NaN) in some columns; preparation will be necessary to deal with these items.
(c)Seasonal Patterns: The data may show seasonal trends and patterns that correspond to year-round fluctuations in the weather.
(d)Possible Outliers: Extreme values or outliers may occur in some variables, indicating odd weather conditions or inaccurate measurements.

#### ASSUMPTIONS FOR BRIGHTON DATASET
It is possible to assume that the observations in this time series data are evenly spaced in time. In other words, each data point—which is a timestamp—occurs at regular intervals, such hourly or daily. The data is also presumed to be stable, which means that its statistical characteristics, such as mean and variance, do not vary over time. Furthermore, the completeness of the data might be presumed.
