## Introduction
In this project we will try to find an optimal location for a restaurant. This report will be targeted to stakeholders interested in opening an restaurant and school in New York.

We will try to detect locations that are not already crowded with restaurants. We choose some candidate location in Queens New York city.
We want to get the cluster information about the Center Queens, so that we can analyze the cluster. Secondly, it is important that analyze the distribution of the restaurant type in each cluster.

## Data

Based on definition of our problem, factors that will influence our decision are:
 - number of existing restaurants in the neighborhood (any type of restaurant)
 - number of and distance to Italian restaurants in the neighborhood, if any
 - distance of neighborhood from city center
 - number of school in the neighborhood (any type of school)
 
We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods. This is our data flow:
 - Get the Queens geometry information
 - Calculate candidate geometry information, under the conditions, like ~6 km from Queens center, and each are has 600 meters each circle apart
 - Get the detailed information in each circle by using Foursquare API

We use other packages
-Pandas
-Numpy
-Json
-Geopy
-Matplotlib
-Shapely
-Pyproj
-Sklearn
-Folium
-Requests

## Methodology
We create the data flow to get the data by using API, then extract the schools and the restaurants information.
After extraction, we dive into exploring the data. We use the PCA method to reduce dimensions and analyze the two main components KDE information.

## Result
We can explore the cluster information, so that we can get the initial conclusion.


## Cluster I
 - Fast Restaurant is main type
 - Western Restaurants have the largest market
## Cluster II 
 - Chinese Restaurant is main type
 - Asian Restaurants have the largest market
## Cluster III
 - Fast Food Restaurant is main type
 - The candidate location has mixture restaurant type
 - The candidate location is a good choice to open an Asian restaurant.
## Cluster IV
 - Fast Food Restaurant is main type
 - The candidate location has mixture restaurant type
 - Asian Restaurants and western restaurant are same important type the Asian restaurant is lack of variety. The candidate location is a good choice to open an Asian restaurant
 
 
## Conclusion
We can make a choice that choose the appropriate restaurant type at appropriate candidate location.
 
