# World_Weather_Analysis-

Using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map.

## Overview

Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary.

## Results

> Deliverable 1 

* Directions:
1. Create a new set of 2,000 random latitudes and longitudes.
2. Get the nearest city using the citipy module.
3. Perform an API call with the OpenWeatherMap.
4. Retrieve the following information from the API call:
~ Latitude and longitude
~ Maximum temperature
~ Percent humidity
~ Percent cloudiness
~ Wind speed
~ Weather description (for example, clouds, fog, light rain, clear sky)

5. Add the data to a new DataFrame.
