# python-api-challenge
***What's the Weather Like?***
<div style="text-align:center"><img src="static/images/heatmap.png" width="1000" height="300"/></div>

<b>BACKGROUND</b><br>
Python requests, APIs, and JSON were used to answer the question: "What's the weather like as we approach the equator?"

<b>DETAILS</b><br>
<b>Part I - WeatherPy</b><br>
A Python script was created to visualize the weather of ~500 unique (non-repeat) cities across the world, at varying distances from the equator using Python library Citipy and the OpenWeatherMap API.<br>

First, a series of scatter plots were creted to showcase the following relationships:<br>
- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude<br>

Second, a linear regression was ran on each relationship after separate the cities into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). The following were plotted with a regression line and y = mx + b equation:<br>
- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude<br>

<div align="center"><img src="static/images/beach_sunset_palmtree.jfif" width="500" height="300"/></div>

<b>Part II - VacationPy</b><br>
Using jupyter-gmaps and the Google Places API, weather data was used to plan future vacations.

First, a heat map was created to display the humidity for every city from Part I - WeatherPy.

Next the DataFrame was narrowed down to find my own ideal weather conditions such as:
 - Maximum temperature lower than 80 degrees but higher than 70.
 - Wind speed less than 10 mph.
 - Zero cloudiness.<br>
 
Any rows that didn't contain all three conditions were dropped to find my ideal weather conditions.


Note: Specifications were adjusted to limit the number of rows returned by the API requests to a reasonable number such as 10.

The Google Places API was used to find the first hotel for each city located within 5000 meters of your coordinates.

Hotels were plotted on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country.
<br>
<b>Additional considerations:</b>

 - The analysis was completed using a Jupyter notebook.
 - Matplotlib and Pandas plotting libraries were used.
 - For Part I, a written description of three observable trends based on the data, were included in the Jupyter notebook.
 - Proper labeling of plots, including plot titles (with date of analysis) and axis labels, were included.
 - For best results on the heat map, the maximum intensity value was set to the highest humidity level found in the data set.


