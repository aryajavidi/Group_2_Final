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

From this data, we have made several tables to display these variables. The photos atattched below can be used as visuals of our dataset throughout the stages if its cleaning and preliminary analysis.

### Original Dataset 

![Dataset](https://user-images.githubusercontent.com/69175360/217972232-3676a107-e411-4de0-9bcd-b168f3e1d67c.JPG)

### Data sorted by NYC only

![Data sorted by nyc](https://user-images.githubusercontent.com/69175360/217972285-fdaeb068-1bac-452b-8d32-6f7c217c28eb.JPG)

### Data sorted by NYC only with only the 6 variables being used for analysis present 

![NYC sorted and dropped](https://user-images.githubusercontent.com/69175360/217972345-e5724def-0c74-4251-9c4e-e619c5c12782.JPG)


## Second Analysis of dataset

For our second analysis of our dataset, we decided to use only three variables to apply to our machine learning model. The three variables chosen were 'accommodates',	'bathrooms', and	'location'. Atattched below are visuals of the tables created to display this dataset. This dataset was run through our machine learning model to train the model and check accuracy. 

### Cleaned Dataset

![3 variable table](https://user-images.githubusercontent.com/69175360/217973044-09d7f164-f34d-468c-8f75-f6d562469c7b.JPG)

### Training the model and checking the accuracy

![accuracy](https://user-images.githubusercontent.com/69175360/217973058-c90b5b7d-f435-4ef3-b541-6487c552dbe9.JPG)


## The questions that the team plans to answer with the project (20 points)

* “Does the number of people an air bnb accommodates affect its price”
 
* “What city is the most expensive to rent an Air BnB in on average?”

* “What is the predicted price of an Air BnB in New York City?”

* "What is the precited price of an Air BnB based on the th enumber of bedrooms"

* "what is the predicted price of an Air BnB that accommodates two"
