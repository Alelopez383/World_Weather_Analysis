# World Weather Analysis
Helping PlanMyTrip, a leading travel technology company, analyze and visualize data for a new project on global weather analysis.
After a Beta test, the customers recommended a few changes to the app like adding the weather description to the weather data; after all, we want to attract more customers, so for this we need to know and be better identify possible nearby travel destinations and corresponding hotels.

Therefore, we need to retrieve the Weather Data; create a Customer Travel Destination Map; an create a Travel Itinerary Map.

## Retriving Weather Data
First, we are going to generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with OpenWeatherMap. In addition, we are going to retrieve the next data: City, country, Date, Latitude and longitude, Maximum temperature, Humidity, Cloudiness, Wind speed, and the current weather description for each city.

Using the OpenWeatherMap API, we found 683 cities after making 2000 calls. As requested at the current time, the weather condition was scattered clouds, regardless of the latitude-longitude; this derives from the fact that when Autumn begins in the Northern Hemisphere and Spring begins in the Southern Hemisphere, the climate is not stable and coud be cloudy. So, the recommendation of the beta testers could not be the best if we only evoke the state of the weather at the current time they perform the search. So, having the most current data in this case is not the most convenient. But it will be great, if we could give a weekly estimate.

![image](https://user-images.githubusercontent.com/43974872/193771076-2c66a4e2-1e97-4674-a73f-01151e4efde2.png)


## Customer Travel Destination Map
Now, of the 683 cities founded, we retrieve the information of 179 cities with their respective hotels, which are the first result of the s search engines in Google.

![image](https://user-images.githubusercontent.com/43974872/193771466-bb958edb-7360-44fe-83a7-9f0d69815e87.png)

We created a heatmap with a pop-up markers with the name of the hotel, city, country code, and the current weather information for each city. One recommendation might be to include the hotel's website or another way to contact them. And a price range per room per night.

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/43974872/193771865-d16ea5a4-b9c0-403e-a33d-0a9930d4544f.png)

## Travel Itinerary
Beta testers were only prompted for weather preference, max and min temp. With these data, the base was filtered and four cities were shown for a possible itinerary. However, preference weather information alone cannot identify potential travel destinations and nearby hotels. Therefore, it is recommended to make more requests for search criteria to improve the results and that these are the closest to the "ideal" of the client.

Now, at the time of creating a travel itinerary. to achieve the best travel route between the four cities, we find that the means of transport is not specified in the pop-up, nor is it mentioned that said route is the best to connect the cities.

![Vacation_travel_map](https://user-images.githubusercontent.com/43974872/193774644-6a34aa3c-e66e-4788-8e3b-9db39398ec25.png)
![Vacation_travel_map_markers](https://user-images.githubusercontent.com/43974872/193774705-c976bb71-663d-4ee1-9616-aaf9957b16f1.png)

# Overview of the Project
## How might we provide real-time suggestions for our client's ideal hotels? 

1. One way to provide real-time suggestions for our client's ideal hotels would be to providing around +/-3 day weather forecasts, or even a weekly forecasts, to avoid weather mishaps; as providing status at the current time of the weather conditions is not very efficient as customers plan their trips in advance. Let´s remember that the weather is no longer as predictable as it used to be, or seasonable.
2. Include forms with more questions to improve the search and the information of the hotels.
3. Include contact information for the hotels, as well as the price range per night and room.
4. Specify the type of transport for the route between cities and show the best option, with transfer times.

