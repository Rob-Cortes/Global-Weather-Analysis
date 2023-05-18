# python-api-challenge

## Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

### Part 1: WeatherPy
This deliverable creates a Python script to visualize the weather of over 500 cities of varying distances from the equator. It uses the citipy Python library and the OpenWeatherMap API to create a representative model of weather across cities.

First, we create plots to showcase the relationships between different weather variables, as shown in the following example:

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/0efc95c4-4524-44ed-8a2d-15002e695610)

Next, we compute a linear regression for each relationship. Given the non-linearity of the plot above, the regressions are separated into Northern Hemisphere and Southern Hemisphere.

Next, create a series of scatter plots, including the linear regression line, the model's formula, and the r-values, as seen in the following example:

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/86b5d252-8f8d-482b-9534-58f5661b7de7)

After each pair of plots are descriptions of each relationship and other findings.

### Part 2: VacationPy
This deliverable makes use of the geoViews Python library and the Geoapify API to create map visualizations.

First, we create a map that displays a point for every city in the city_data_df DataFrame as shown in the image below. The size of the points scale with the humidity in each city.

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/bcc05bfa-3531-4c15-9ccc-70ba854d899d)

Next, we narrow down the city_data_df DataFrame to find ideal weather conditions, and create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, we use the Geoapify API to find the first hotel located within 10,000 meters of the city's coordinates, and add the hotel name and the country as additional information in the hover message for each city on the map.

![image](https://github.com/Rob-Cortes/python-api-challenge/assets/124944383/a93afffb-9571-4975-ae67-d9d48e6d49d2)
