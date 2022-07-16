# World Weather Analysis

## Overview of World Weather Analysis

Plan My Trip is top online travel company that specializes in the hotel and lodging industry.  Jack, the head of analysis of the user interface team at Plan My Trip, engaged me to help him collect and present data for customers via the search page.  The customers will filter their searches based on their preferred travel criteria in order to find their ideal hotel anywhere in the world. 
 
### Resources

* Data Source:  city_data.csv, ride_data.csv
* Software:  Python 3.6.1, Jupyter Notebook (anaconda3), Visual Studio Code 1.38.1
* Packages:  Pandas, NumPy, Gmaps, Matplotlib, and CityPy

## World Weather Analysis Methdology

To perform this task, we used the CityPy module to obtain more than 600 cities across the globe using 2,000 randomly generated latitudes and longitudes.  Using the Open Weather Map API, we retrieved the json weather data for each city by name.  The weather data was added to a pandas dataframe, so we could explore the relationships between all of the cities' latitudes and their weather using Matplotlib graphs.

Once the statistical analyses were performed, we created an input script to obtain the travel preferences for each customer.  We used the customer's travel preferences to filter the cities dataset.  Then, we used the Google Places API to create a list of hotels near each city returned for each customer's travel preferences.  Once the hotel data was incoporated into our dataframe, we used the Google Maps API to plot each hotel on a map for the customers to see.

We then used the Google Directions API to chart out the travel itinerary for a particular customers trip.  That information included pins for each destinatation and a list of hotels and current weather for each location.

### Pictures of final results

World Weather Search Map:
![WeatherPy_Vacation_Map.png](Vacation_Search/WeatherPy_Vacation_Map.png)

Sample Travel Itinerary Map:
![WeatherPy_Travel_Map.png](Vacation_Itinerary/WeatherPy_Travel_Map.png)

Sample Travel Itinerary Map with Markers:
![WeatherPy_Travel_Map_Markers.png](Vacation_Itinerary/WeatherPy_Travel_Map_Markers.png)

## Code Snippets

Open Weather Map API Call:
![OpenWeatherMap_API_Call.png](weather_data/OpenWeatherMap_API_Call.png)

Statistical Analysis on Temperatures by Hemisphere:
![Statistical_Analysis_Temp.png](weather_data/Statistical_Analysis_Temp.png)

Customer Input Filter:
![Customer_Input_Filter.png](weather_data/Customer_Input_Filter.png)

Hotel API Search:
![Hotel_API_Search.png](weather_data/Hotel_API_Search.png)

World Weather Map Script:
![World_Weather_Map_Script.png](weather_data/World_Weather_Map_Script.png)

Itinerary Map Script:
![Itinerary_Map_Script.png](weather_data/Itinerary_Map_Script.png)

Itinerary Marker Map Search:
![Itinerary_Marker_Map_Script.png](weather_data/Itinerary_Marker_Map_Script.png)
