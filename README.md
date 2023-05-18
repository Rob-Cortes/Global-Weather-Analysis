# python-api-challenge

## Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

### Part 1: WeatherPy
This deliverable creates a Python script to visualize the weather of over 500 cities of varying distances from the equator. It uses the citipy Python library and the OpenWeatherMap API to create a representative model of weather across cities.

First, we create plots to showcase the relationships between the following variables:

Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

Next, we compute a linear regression for each relationship. The plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).

Next, create a series of scatter plots, including the linear regression line, the model's formula, and the r-values, as seen in the following image:

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/33e59f03-8000-4868-b96c-8f24e687eaf7)

Lastly, we create the following plots:

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots are descriptions of each relationship and other findings.

### Part 2: VacationPy
This deliverable makes use of the geoViews Python library and the Geoapify API to create map visualizations.

First, we create a map that displays a point for every city in the city_data_df DataFrame as shown in the image below. The size of the points scale with the humidity in each city.

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/fe1c508c-582c-4573-9304-532da0cf2691)

Next, we narrow down the city_data_df DataFrame to find ideal weather conditions, and create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, we use the Geoapify API to find the first hotel located within 10,000 meters of the city's coordinates, and add the hotel name and the country as additional information in the hover message for each city on the map.
