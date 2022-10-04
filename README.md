# World Weather Analysis
Helping PlanMyTrip, a leading travel technology company, analyze and visualize data for a new project on global weather analysis.
After a Beta test, the customers recommended a few changes to the app like adding the weather description to the weather data; after all, we want to attract more customers, so for this we need to know and be better identify possible nearby travel destinations and corresponding hotels.

Therefore, we need to retrieve the Weather Data; create a Customer Travel Destination Map; an create a Travel Itinerary Map.

## Weather Data
First, we are going to generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with OpenWeatherMap. In addition, we are going to retrieve the next data: City, country, Date, Latitude and longitude, Maximum temperature, Humidity, Cloudiness, Wind speed, and the current weather description for each city.

# Overview of the Project
At the most fundamental level, we want to answer: 
- How might we provide real-time suggestions for our client's ideal hotels? Y
- What is the "ideal"? In a first glampse we´ll narrow it to hotels that are within a given range of latitude and longitude and that provide the right kind of weather for the client.
