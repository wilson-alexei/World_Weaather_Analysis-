# World_Weather_Analysis-

Using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map.

## Overview

Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary.

## Deliverable 1

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

* Results:

<img width="647" alt="D1-1" src="https://user-images.githubusercontent.com/95068439/166129459-9bd9f7b1-7a58-4cd4-80ae-f3d5e32f8517.png">

<img width="1204" alt="D1-2" src="https://user-images.githubusercontent.com/95068439/166129461-ff4dce50-ed7d-4ff8-b64f-c11c85032a9d.png">

<img width="1224" alt="D1-3" src="https://user-images.githubusercontent.com/95068439/166129463-042584a0-6362-47a7-a0b6-5eda07515eb8.png">

## Deliverable 2

* Directions: 
1. Import the `WeatherPy_Database.csv` file from your `Weather_Database` folder from Deliverable 1 as a DataFrame.

2. Write two input statements that prompt the user to enter their minimum and maximum temperature criteria for their vacation.

3. Use the `loc` method to filter the `city_data_df` DataFrame for temperature criteria collected in Step 2, then create a new DataFrame.

4. Determine if there are any empty rows, then drop them if necessary and create a new DataFrame.

5. Use the provided code to create a new DataFrame, `hotel_df`, that will hold the hotel names from the hotel search in Steps 6a-6f.

6. Iterate through the `hotel_df` DataFrame, retrieve the latitude and longitude of each city to find the nearest hotel based on the search parameters, then add the hotel name to the `hotel_df` DataFrame. If a hotel isn't found, skip to the next city.

7. Drop any rows in the `hotel_df` DataFrame where a hotel name is not found.

8. Create an output file to store the `hotel_df` DataFrame as `WeatherPy_vacation.csv` in the Vacation_Search folder.

9. Add the city name, the country code, the weather description, and the maximum temperature for the city to the `info_box_template` format template we have provided.

10. Use the provided list comprehension code to retrieve the city data from each row, which will then be added to the formatting template and saved in the `hotel_info` list.

11. Use the provided code snippet to retrieve the latitude and longitude from each row and store them in a new DataFrame.

12. Refactor your previous marker layer map code to create a marker layer map that will have pop-up markers for each city on the map.

* Results: 

<img width="876" alt="D2-1" src="https://user-images.githubusercontent.com/95068439/166129606-40dd9e1d-4e7f-4c32-af09-1fae681ee50f.png">

<img width="993" alt="D2-2" src="https://user-images.githubusercontent.com/95068439/166129608-d322e397-b766-43ac-be6c-95309b944ef1.png">

<img width="954" alt="D2-3" src="https://user-images.githubusercontent.com/95068439/166129609-98af535b-c197-403f-898b-d3daf0f927b7.png">

<img width="909" alt="D2-4" src="https://user-images.githubusercontent.com/95068439/166129610-fab89f4f-909c-4f40-a728-7b06003557f7.png">

<img width="803" alt="D2-5" src="https://user-images.githubusercontent.com/95068439/166129611-1c1cb506-f5bd-4dff-92c0-cbe873e95e37.png">

<img width="1038" alt="D2-6" src="https://user-images.githubusercontent.com/95068439/166129612-8053ceaa-e425-459f-b439-b519eedf8f82.png">

## Deliverable 3

* Directions:
1. Import the WeatherPy_vacation.csv file from your Vacation_Search folder from Deliverable 2 as a DataFrame.

2. Create a marker layer map of the vacation search results.

3. From the vacation search map, choose four cities that a customer might want to visit. They should be close together and in the same country.

4. Use the variables we have provided and the loc method to create separate DataFrames for each city on the travel route.

5. Use the `to_numpy()` function and list indexing to write code to retrieve the latitude-longitude pairs as tuples from each city DataFrame.

6. Create a directions layer map using the variables from Step 6, where the starting and ending city are the same city, the waypoints are the three other cities, and the travel_mode is either `"DRIVING"`, `"BICYCLING"`, or `"WALKING"`.

7. Use the provided concat() function code snippet to combine the four separate city DataFrames into one DataFrame.

* Results: 

<img width="842" alt="D3-1" src="https://user-images.githubusercontent.com/95068439/166130011-7428b752-c259-44f5-b555-b9139e8e9376.png">

<img width="929" alt="D3-2" src="https://user-images.githubusercontent.com/95068439/166130016-49ba9a68-e019-43cf-8b3f-cc98328c8cfe.png">

<img width="962" alt="D3-3" src="https://user-images.githubusercontent.com/95068439/166130018-b0c2e5cf-2979-4b1a-af3a-c4b099a73c93.png">

<img width="1008" alt="D3-4" src="https://user-images.githubusercontent.com/95068439/166130021-120c14ba-ce42-439a-92e9-6ba6a11bfa47.png">

<img width="1020" alt="D3-5" src="https://user-images.githubusercontent.com/95068439/166130023-4e51a6f2-5d20-4eb1-91eb-1d958d784b6f.png">

* Map Itinerary 

![WeatherPy_travel_map](https://user-images.githubusercontent.com/95068439/166130062-4d32a82d-92aa-417a-b2e8-55d04b8e694f.png)

![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/95068439/166130069-3a0f0435-a1d6-4a6f-bdd0-dff7bf65ba9e.png)

> LinkedIn: https://www.linkedin.com/in/wilson-alexei/

> Email: wils.alexei@gmail.com
