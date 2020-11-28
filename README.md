# Python API Challenge: Weather API #

## Objectives ##

#### WeatherPy ####

Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator, utilizing CitiPy and the OpenWeatherMap API.
Create a series of scatter plots to showcase the following relationships:

- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

Run a linear regression on each relationship, separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- ...

1. Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
2. Perform a weather check on each of the cities using a series of successive API calls.
3. Include a print log of each city as it's being processed with the city number and city name.
4. Save a CSV of all retrieved data and a PNG image for each scatter plot:
  - The retrieved data is stored in output_data.csv
  - the scatter plots can be found in the images folder as well as in the WeatherPy notebook with included commentary on possible linear relationships.

#### VacationPy ####

1. Create a heat map that displays the humidity for every city from the part I (WeatherPy).
2. Narrow down the DataFrame to find your ideal weather condition.
3. Use Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
4. Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

All of these steps are executed within the VacationPy notebook. 

#### Important! ####
To run the code, you will need all of the dependencies installed, as well as a key for the OpenWeatherMaps and Google gmaps APIs. Additionally, you will need to input these keys into the `w_api` and `g_api` variables in the config.py file in each folder.
