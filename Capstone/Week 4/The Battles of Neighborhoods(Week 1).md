## The Battles of Neighborhoods

### 1 Introduction|Business Problem

This project aims to help people exploring better facilities around their neighbourhoods, which will help people to get awareness of the area and neighborhood before moving to a new city, state, country or place for their work or to start a new fresh life, in this project, Scarborough in Toronto.

As lots of people are migrating to various states of Canada and need to do lots of research in order to find the proper neighbourhood environment. For example, proper housing prices, reutated schools, supermarket, hospital, etc. This project is to meet this kind of demand.



### 2 Data Description

#### 2.1 Data

Data Link: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

For this dataset, we used the York dataset that  scrapped from wikipedia. The dataset consisting of latitude, longtitude and zip codes.



#### 2.2 Foursquare API Data:

We will need data about different venues in different neighborhoods of that specific borough. In order to gain that information we will use "Foursquare" locational information. Foursquare is a location data provider with information about all manner of venues and events within an area of interest. Such information includes venue names, locations, menus and even photos. As such, the foursquare location platform will be used as the sole data source since all the stated required information can be obtained through the API.

After finding the list of neighborhoods, we then connect to the Foursquare API to gather information about venues inside each and every neighborhood. For each neighborhood, we have chosen the radius to be 100 meter.

The data retrieved from Foursquare contained information of venues within a specified distance of the longitude and latitude of the postcodes. 



### 3 Methods and Tools 

#### 3.1 Foursquare API

The Foursquare API will be used for this project as its prime data gathering source. Because it has a database of millions of places and it provides the service to perform location search, location sharing and details about a business.

#### 3.2 Clustering Approach

In order to compare the two cities, we decided to use k-means clustering algorithm to cluster data. Additionally, we will explore, segment and group the  neighborhoods into clusters to find similar neighborhoods in a big city, for example, New York and Toronto.

#### 3.3 Libraries

Pandas: For creating and manipulating dataframes.

Beautiful Soup and Requests: To scrap and library to handle http requests.

Geocoder: To retrieve Location Data.

Folium: Python visualization library would be used to visualize the neighborhoods cluster distribution of using interactive leaflet map.

XML: To separate data from presentation and XML stores data in plain text format.

Scikit Learn: For importing k-means clustering.

Matplotlib: Python Plotting Module.

JSON: Library to handle JSON files.



