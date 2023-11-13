# Amsterdam
Analysis of Airbnb listings data in Amsterdam 2018.

## Context
Amsterdam, the capital of the Netherlands, is known for its picturesque canals, historic architecture and diverse cultural offerings.  In this case study we will delve into the relationship between  properties listed here on Airbnb, a popular online marketplace for short-term accomodation rental. 
With 20030 properties listed on Airbnb in Amsterdam, hosts may need some guidance to compare their pricing against similar properties. This dashboard should serve as a helpful tool. 

## Motivation
As someone who is interested in travel around Europe, this data set stood out to me as the starting point for my analysis. I have chosen it because it meets the criteria necessary for me to further my skills in the areas of:
* Geographical visualizations with python
* Supervised Machine Learning: Regression
* Unsupervised Machine Learning: Clustering
* Time Series Analysis
* Creating Data Dashboards

## The Dataset
This is a group of files comprising of data made publicly available by AirBnB. I downloaded this
data set from [kaggle on November 1st, 2023](https://www.kaggle.com/datasets/erikbruin/airbnb-amsterdam?select=reviews_details.csv). The files are downloaded from insideairbnb.com
and give a snapshot of the Amsterdam situation on December 6th, 2018
Airbnb is an online company that runs a marketplace for temporary rentals and homestays for
vacation, and tourism activities. Based in San Francisco, California, the platform is accessible
via website and mobile app. Airbnb does not own any of the listed properties; instead, it
profits by receiving commission from each booking.
### Data Contents:
The set is made-up of 7 files (6 .csv and 1 .geojson) as outlined below:
#### calendar.csv
contains 365 records for each listing. It specifies whether the listing is available on a particular
day (365 days ahead), and the price on that day. Its columns are:
listing_id, date, available, price
#### listings.csv
A listing is basically and advertisement for the property. This file holds the most useful
variables from the property listings on December 6th, 2018:
id, name, host_id, host_name, neighbourhood_group, neighbourhood, latitude, longitude,
room_type, price, minimum_nights, number_of_reviews, last_review, reviews_per_month,,
calculated_hot_listings_count, availability_365
#### listings_details.csv
this file holds the same variables as listings.csv plus 80 additional variables.
#### neighbourhoods.csv
contains one empty column, and one containing 22 names of Amsterdam neighbourhoods in
Dutch.
#### reviews.csv
This is a simple file that can be used to count the number of reviews by listing (for a specific
period). It only has 2 columns:
listing_id, date
#### reviews_details.csv
This file holds the full details of all reviews with 6 columns:
listing_id, id, date, reviewer_id, reviewer_name, comments
#### neighbourhoods.geojson
The shape file that can be used in conjunction with interactive maps (such as the Python
folium package)

## Limitations & Ethics
Being pulled from 2018, this data will be a little old to draw any real-world predictions of the
state of the AirBnB market today. It will however present an adequate opportunity to develop
the necessary skills.
The data contains potential PII. The names of hosts and users will not be necessary for the
scope of my project and can be removed accordingly.
The information will be more usable for me in analysis once I combine the relevant columns
from the existing tables into a larger dataframe. 

## In this Respository

* Project Management: Contains the Project Brief
  
* Scripts: Contains all the Jupyter Notebooks of Python coding for the analysis

*  README outlines project

## Links

[Tableau Storyboard](https://public.tableau.com/views/AmsterdamBnB_16996240579480/Story1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)
