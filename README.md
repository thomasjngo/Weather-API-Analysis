# Summary

## Part 1: WeatherPy

In this project, a Python script was developed to visualize the weather across over 500 cities at varying distances from the equator. Utilizing the `citipy` library and the OpenWeatherMap API, weather data was retrieved to create a representative model of weather conditions across these cities.

### Key Tasks

1. **Weather Variables vs. Latitude Plots**
   - Weather data for the cities was retrieved using the OpenWeatherMap API.
   - Scatter plots were created to showcase the relationships between latitude and various weather variables:
     - Temperature
     - Humidity
     - Cloudiness
     - Wind Speed

2. **Linear Regression Analysis**
   - Linear regression was computed for each relationship.
   - Separate plots were created for the Northern Hemisphere (≥0 degrees latitude) and Southern Hemisphere (<0 degrees latitude).
   - Each scatter plot included the linear regression line, model formula, and r² values.
   - Detailed analysis was performed for the following plots:
     - Northern Hemisphere: Temperature vs. Latitude
     - Southern Hemisphere: Temperature vs. Latitude
     - Northern Hemisphere: Humidity vs. Latitude
     - Southern Hemisphere: Humidity vs. Latitude
     - Northern Hemisphere: Cloudiness vs. Latitude
     - Southern Hemisphere: Cloudiness vs. Latitude
     - Northern Hemisphere: Wind Speed vs. Latitude
     - Southern Hemisphere: Wind Speed vs. Latitude
   - Observations and findings from the linear regression models were documented.

## Part 2: VacationPy

This part of the project involved using weather data to plan future vacations by creating map visualizations with the `geoViews` library and the Geoapify API.

### Key Tasks

1. **City Map Creation**
   - A map was created displaying a point for each city in the `city_data_df` DataFrame, with the point size representing the humidity in each city.

2. **Ideal Weather Condition Filtering**
   - The `city_data_df` DataFrame was filtered to find cities with ideal weather conditions, such as:
     - Maximum temperature between 21 and 27 degrees Celsius
     - Wind speed less than 4.5 m/s
     - Zero cloudiness
   - The specifications were adjusted to ensure a reasonable number of rows returned by API requests.

3. **Hotel DataFrame Creation**
   - A new DataFrame (`hotel_df`) was created to store city, country, coordinates, and humidity data.
   - The Geoapify API was used to find the first hotel within 10,000 meters of each city’s coordinates.
   - The hotel names and countries were added to the map's hover message for each city.

The project successfully demonstrated the use of Python for data visualization and analysis, utilizing various APIs and libraries to create meaningful insights and visual representations.
