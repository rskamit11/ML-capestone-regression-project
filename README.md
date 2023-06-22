# ML-capestone-regression-project
Project title : Seoul Bike sharing Demand Prediction
Problem Statement :
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

Project Summary :
These dataset contains hourly and daily count of the rental bikes count  between year 2017 and 2018 in capital bike share systems with corresponding weather and seasonal information.The dataset contains 8760 rows for every hour of the each day for 2017 and 2018 and 14 columns for features which are under  consideration. The dataset contain weather information such as temperature, humidty, snowfall, rainfall, windspeed , visibility, dew point, solar radiation the number of the rented per hour and date information. Bike sharing gaining importance last few year over last few decades. More and more people are turning more healthier and liveable cities where activities like bike sharing are easily available there are many benefits of bike sharing such as enviromental benefits, it also help us in maintaining physical health active.

Important Library :
Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

Statsmodels: For statistical computations

Dataset information :
Date - The date of each observation in the format 'year-month-day'

Hour - Hour of the day

Temperature - Temperature recorded in the city in Celsius (°C).

Humidity - Relative humidity in %

Wind speed - Speed of the wind in m/s

Visibility - measure of distance at which object or light can be clearly discerned in units of 10m

Dew point temperature - Temperature recorded in the beginning of the day in Celsius(°C).

Solar radiation - Intensity of sunlight in MJ/m^2

Rainfall - Amount of rainfall received in mm

Snowfall - Amount of snowfall received in cm

Seasons - Season of the year (Winter, Spring, Summer, Autumn)

Holiday - Whether the day is a Holiday or not (Holiday/No holiday)

Functional Day -Whether the rental service is available (Yes-Functional hours) or not (No-Non functional hours)

Exploratory Data Analysis :
Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

Feature engineering and data preprocessing :
Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.
Created new columns such as Day, Month, Year, Days_of_week and Weekend from Date column .
Checked the VIF value (measure of multicollinearity) and dropped Dew point Temperature and Year which were highly correlated with other independent features.
The categorical features present in the dataset Seasons, Holiday, Weekend, Functioning Day were dummified.
Brought features to a similar range using MinmaxScaler.

ML model implementation :
Implementation of Regression models
Linear Regression

Polynomial Regression

Decision Tree

Random Forest

XGBoost

Hyperparameter tuning :

Conclusion :
Most number of bikes are rented in the Summer season and the lowest in the winter season.Over 96% of the bikes are rented on days that are considered as No Holiday.Most number of bikes are rented in the temperature range of 15 degrees to 30 degrees.Most number of bikes are rented when there is no snowfall or rainfall.Majority of the bikes are rented for a humidity percentage range of 30 to 70.The highest number of bike rentals have been done in the 18th hour, i.e 6pm, and lowest in the 4th hour, i.e 4am.Most of the bike rentals have been made when there is high visibility.
XG boost Regression is the best performing model with an r2 score of 0.926.
SVR is the worst performing model with an r2 score of 0.221.Temperature and Hour are the two most important factors according to all the models.



