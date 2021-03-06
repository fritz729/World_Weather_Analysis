# Weather Analysis

## Summary

This project use API's to gather weather data for a selection of cities based on the latitude and longitude that are randomly generated.  The set is used to identify cities using the 'citipy' module and using this data, collect the weather data from the city using openweatherapi.org.  This allows us to create a DataFrame containing the weather data that can be used to select cities that meet the users temperature range for planning a vacation.  The dataset is filtered for the cities that meet the users temperature range and presents a map showing the cities that meet the criteria and hotels at each destination.  From this list the user can select a round trip within an area limited to a starting city and 3 destinations which return back to the starting city.

---

## Results

### Data set creation and filter

For the trial dataset we created a dataframe containing cities selected from a random generation of 2000 longitude and latitude combinations.  This created a data set of 550 cities that were unique around the globe. This dataset would provide the information to select and create the travel itinerary. For this dataset we used a range between 75F and 95F.  This gave us a set of 164 cities that met the criteria.  These cities were marked on the map as seen below:

<img src="Vacation_Search/WeatherPy_vacation_map.png" width="680" height="300">

### Travel itinerary and route creation

To create the travel itinerary the user selects 4 cities from the dataset with the starting city also being the ending city.    Once selected and entered into the code the route map is created using gmaps API.  This map then has markers placed on the cities that were selected and information on each city is available when the marker is selected.  Examples of the maps created are shown below:

#### Route map

<img src="Vacation_Itinerary/WeatherPy_travel_map.png" width="800" height="300">

#### Marker map

<img src="Vacation_Itinerary/WeatherPy_travel_map_markers.png" width="800" height="800">

---

## Conclusion

This project shows how the use of API's can access a wide range of data and allow users to filter and sort the data in a meaningful way using some basic code.  

---
