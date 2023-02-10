# Group_2_Final


## The selected topic and the reasoning for that selection (20 points)

Group two consists of Jessica Cobb, Ranil Basnayake, Zach Otto, and Arya Javidi. The topic we have chosen to analyze is AirBnB data. We plan to use machine learning to predict the prices of AirBnB rentals in different cities based on property type, number of people it can accommodate, number of bedrooms and bathrooms, and the city in which it is located. The locations that we aim to predict the price of Airbnb listings in are six major cities in US: New York city, Los Angeles,  San Francisco, Washington DC, Chicago, and Boston.


## A description of the data (20 points)

The data we are working with was retrieved from Kaggle from the [following link](https://www.kaggle.com/datasets/rudymizrahi/airbnb-listings-in-major-us-cities-deloitte-ml/).

The data was provided as a part of the Deloitte Machine Learning Competition. The data was provided in CSV format. There are 74,112 rows and 29 columns, which we have reduced to 6 columns after determining which variables would be most pertinent to our machine learning model and analysis.

### The dataset originally contained the following variables: 
* id
* log_price
* property_type
* Room_Type
* Amenities
* Accomodates
* Bathrooms
* Bed_type
* cleaning_fee
* city
* host_identity_verified
* instant_bookable
* latitude
* longitude
* neighbourhood
* number_of_reviews
* cancellation_policy
* review_scores_rating
* zipcode
* bedrooms
* beds
* Cancellation Policy
* Description
* Host Profile Pic
* Host Response
* Host Since
* First Review
* Last Review
* Name
* thumbnail_url

### The variables we have decided to analyze are 

* room_type
* accommodates
* neighbourhood
* zipcode
* bedrooms
* bathrooms

We dropped variables from the dataset because we felt that they did not have a significant impact on our goal and results. Variables such as, "name" and "description" would be difficult for our machine learning model to draw conclusions from. 

## The questions that the team plans to answer with the project (20 points)

* “Does the number of people an air bnb accommodates affect its price”
 
* “What city is the most expensive to rent an Air BnB in on average?”

* “What is the predicted price of an Air BnB in New York City?”
