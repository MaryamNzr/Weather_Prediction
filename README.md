# Weather_Prediction

### Background
The goal is to develop an accurate and reliable weather prediction model using time series data. The goal is to leverage data science techniques to forecast weather conditions for a given location, enabling individuals and organizations to make informed decisions and plan activities accordingly.The challenge lies in capturing and analyzing historical weather data, understanding the patterns, and developing a predictive model that can effectively forecast future weather conditions. Factors such as temperature, humidity, wind speed, and precipitation are considered to create a comprehensive prediction system.

![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/Pic1.jpeg)
### The Data
The [dataset](https://www.kaggle.com/datasets/ananthr1/weather-prediction?sort=published)from Kaggle consisted of 1461 days. The contents included information such as; precipitation, max temperature, min temperature, wind speed, and weather condition. Numeric metrics included information like wind speed, max and min temprature. I cleaned and wrangled the data in preparation for time series analysis. Since this is a TimeSeries problem, I had to parse 'date' column. The code for this step is contained in the Notebooks folder (https://github.com/MaryamNzr/Weather_Prediction/blob/main/Weather_Prediction_Data_Wrangling%26EDA.ipynb).
### Data visualization
Features:
Precipitation
Wind
Date
Target:
Temperature
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/pic2.png)
### Pre-processing
Check the Chronological Order:
The data should be in chronological order and the timestamps should be equidistant in time series. The chronological order is achieved by sorting the dataframe by the timestamps. Equidisant timestamps indicates constant time intervals. To check this, the difference between each timestamp is taken. The code is contained in the Notebooks folder, titled [Preprocessing](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Weather_Prediction_Data_TimeSeries_EDA.ipynb).
#### Smoothing Data / Resampling
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/3.png)
#### Stationary
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/4.png)
#### TimeSeries Decomposition
Time series decomposition involves thinking of a series as a combination of level, trend, seasonality, and noise components.
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/5.png)
### Exploratory Data Analysis
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/6.png)
As we can see Temperature reaches its maximum around May/June and its minimum around November Wind: reaches its maxmium around August and its minimum around January Precipitation: reaches its minimum around July
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/7.png)
### Autocorrelation Analysis
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/8.png)

### Modeling
Cross Validation
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/9.png)
#### Models for Univariate Time Series
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/10.png)
#### ARIMA
![This is an image](https://github.com/MaryamNzr/Weather_Prediction/blob/main/Images/11.png)


