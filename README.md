# Python API Homework - What's the Weather Like?

# Introduction
This analysis looked at weather by cities around the world. The weather data was ultimately used to plan desirable location destinations.
# Overview
Citypi generated a set of world wide cities with latitude/longitude. measurements. OpenWeatherMap was used to get the corresponding weather conditions. The results were graphed on specific weather characteristics. The second part of the assignment used heat maps to look at humidity. Then city choices were narrowed down based on the most desireable characteristics.
# Methodology
Citypi was used to generate 500+ cities world wide and their latitude and longitudes. OpenWeatherMap was used to get current weather conditions on these cities. This was done with an API call based on the latitude and longitude. The results were put in a dataframe and graphed with scatter plots. The first part graphed latitude against: max temperature, humidity, cloudiness, and wind speed. The second part was regression analysis of the norther hemisphere vs the southern hemisphere in latitude versus: max temperature, humidity, cloudiness, and wind speed. 

# Analysis
The scatter plots appear to be very random for latitude against: max temperature, humidity, cloudiness, and wind speed.
![latitude vs temperature](WeatherPy\Images\1.png)<br />
![latitude vs humidity](WeatherPy\Images\2.png)<br />
![latitude vs cloudiness](WeatherPy\Images\3.png)<br />
![latitude vs windspeed](WeatherPy\Images\4.png)

Once the data sets are split into northern and southern hemisphere, correlation is evident. Temperature effects a strong correlation; with the northern hemisphere being negatively correlated to latitude and the southern hemisphere having a strong positive correlation. : <br /> 
![regression northern](WeatherPy\Images\5.png)<br />
![regression southern](WeatherPy\Images\6.png)<br />

The regression of humidity versus latitude has postive correlation for the northern hemisphere; while the southern hemisphere has a flat to slightly positive correlation with humidity:<br />
![regression northern](WeatherPy\Images\7.png)<br />
![regression southern](WeatherPy\Images\8.png)<br />

The regression of latitude versus cloudiness is similar to that of humidity.  The northern hemisphere has a  postive correlation for cloudiness; while the southern hemisphere has a flat to slightly positive correlation:<br />
![regression northern](WeatherPy\Images\9.png)<br />
![regression southern](WeatherPy\Images\10.png)<br />

Lastly we have a comparison of Latitude to wind speed.
Similar to the temperature results, it can be seen that wind speed is positively correlated to latitude, while in the southern hemisphere, there is a negative correlation to wind speed.

![regression northern](WeatherPy\Images\11.png)<br />
![regression southern](WeatherPy\Images\12.png)<br />

# Conclusions
There are a couple of points to keep in mind while looking at this data.  It is a random sampling of cities, and there are parts of the world without cities. It is a snapshot in time, with the weather conditions given only for the day requested. lastly, the earth has a tilt, so one hemisphere is always closer to the sun than the other. With these factors in mind, this graph and data could be used to identify possible places to travel to depending on your own preferences of temperature, etc. However, that predictive value would only be good for, right not or this particular season for which the data was collected.  The weather conditions could be very different at other times of year.
