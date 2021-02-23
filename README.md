# python-api-challenge
***What's the Weather Like?***

BACKGROUND<br>
Using Python requests, APIs, and JSON to answer the question: "What's the weather like as we approach the equator?"

DETAILS<br>
Part I - WeatherPy<br>
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

Part II - VacationPy<br>
Using jupyter-gmaps and the Google Places API, weather data was used to plan future vacations.

First, a heat map was created to display the humidity for every city from Part I - WeatherPy.

Next the DataFrame was narrowed down to find my own ideal weather conditions such as:
 - Maximum temperature lower than 80 degrees but higher than 70.
 - Wind speed less than 10 mph.
 - Zero cloudiness.<br>
 
Any rows that didn't contain all three conditions were dropped to find my ideal weather conditions.


Note: Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number like 10.




The Google Places API was used to find the first hotel for each city located within 5000 meters of your coordinates.


Hotels were plotted on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country.



As final considerations:

You must complete your analysis using a Jupyter notebook.
You must use the Matplotlib or Pandas plotting libraries.
For Part I, you must include a written description of three observable trends based on the data. You can do this right in the Jupyter notebook.
You must use proper labeling of your plots, including plot titles (with date of analysis) and axis labels.
For best results on the heat map, try setting the the maximum intensity value to the highest humidity level found in the data set.


