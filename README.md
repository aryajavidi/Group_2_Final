# Group_2_Final



## Feb 7th update

This week our team worked together to edit the dataset and remove parts of the dataset that could lead to confusion in our machine learning model. We have chosen which variables will be used in our analysis and which will be dropped.

### The variables that we have chosen to analyze are: 

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



### The following variables were dropped from the dataset:

* Cancellation Policy
* Description
* Host Profile Pic
* Host Response
* Host Since
* First Review
* Last Review
* Name
* thumbnail_url

We dropped these variables because we felt that they did not have a significant impact on our goal, being able to predict the cost of an AirBNB booking based on several variables. Variables such as, "name" and "description" would be difficult for our machine learning model to draw conclusions from. Names such as "BEST HOLLYWOOD LOCATION!!!" and "Spacious Room up to 8 Guests" provide us with the same information that variables such as 'beds' or 'city' could. 



