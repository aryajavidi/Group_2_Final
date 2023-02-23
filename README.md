# Group_2_Final - Predicting AirBnB Rental Prices based on accomodations. 


## The selected topic and the reasoning for that selection 

Group two consists of Jessica Cobb, Ranil Basnayake, Zach Otto, and Arya Javidi. The topic we have chosen to analyze is AirBnB data. We plan to use machine learning to predict the prices of AirBnB rentals in different cities based on property type, number of people it can accommodate, number of bedrooms and bathrooms, and the city in which it is located. 

We have chosen to analyze data regarding Air BnB prices and the variables that may affect that price because short term rentals are becoming a more and more popular option for people that are traveling. Renting a private property is considered by some to be more safe, cost efficient, and fun. This upwards trend in business has led more renters and property owners to be interested in the value of these properties. This model can help a renter decide if an AirBnB is fairly priced or may help a new renter decide on a price to list their property. We also have a special interest in the industry as we have a few prospective buyers in our group as well!


A Link to our presentation can be found [here](https://docs.google.com/presentation/d/14_f2t58X_Ch7xfNvNBw9JvORSmUic1HXzjBF5L6d0oE/edit#slide=id.p1)


## The questions that the team plans to answer with the project 

* “Are certain amenities more valuable in some cities versus others?”

* “Which neighborhood in New York City is the most expensive to rent an Airbnb?”

* “How does the average price of an Airbnb change based on city?” 

* "Which factors influence the cost of an Airbnb the most?"

* “What amenities drive up the price of an Airbnb?”

## A description of the data 

The data is available for free from the following [Kaggle webpage](https://www.kaggle.com/datasets/rudymizrahi/airbnb-listings-in-major-us-cities-deloitte-ml). 

This data was provided originally for the Deloitte Machine Learning Competition.
There are 74,112 rows of data abd 28 columns including 27 features. Our target variable is the log_price of each listing.
The 27 features include Cancellation Policy, Description, Host, Profile Pic, Host Response, Host Since, First Review, Last Review, Name, thumbnail_url, etc.
We dropped variables from the dataset because we felt that they did not have a significant impact on our goal and results. Variables such as, "name" and "description" would be difficult for our machine learning model to draw conclusions from.

We dropped some variables from the dataset because we felt that they did not have a significant impact on our goal and results. Variables such as, "name" and "description" would be difficult for our machine learning model to draw conclusions from without the use of natural language processing which we felt was out of our scope for this project given the timeframe and our experience with the subject.

From this data, we have made several tables to display these variables. The photos atattched below can be used as visuals of our dataset throughout the stages if its cleaning and preliminary analysis.

### Original Dataset 

![Dataset](https://user-images.githubusercontent.com/69175360/217972232-3676a107-e411-4de0-9bcd-b168f3e1d67c.JPG)

## Analysis of dataset


To begin, we had to choose a model that would work for us. We considered four different methods at first, testing each with our dataset and identifying which would be the best fit for our project.

#### Models considered and results of each

![models](https://user-images.githubusercontent.com/69175360/221027253-8f5c7fb5-442a-4463-b2a7-db2368931eb6.JPG)


For our first analysis of our dataset, we decided to use only three variables to apply to our machine learning model. The three variables chosen were 'accommodates',	'bathrooms', and	'location'. 

Atattched below are visuals of the tables created to display this dataset. This dataset was run through our machine learning model to train the model and determine accuracy. We made many revisions to the model over the past few weeks changing which features we would train with and learning how to extract out each amenity in the amenities column to a new column with a True/False output. 

After training the model on the chosen features, we created visualizations to display how the model weighs each feature when predicting the log_price. After training the model on New York and Los Angeles datasets, we created two pie charts to compare how certain amentieies may be weighed more or less depending on which city they were in.


#### Cleaned Dataset

![3 variable table](https://user-images.githubusercontent.com/69175360/217973044-09d7f164-f34d-468c-8f75-f6d562469c7b.JPG)

#### Training the model and checking the accuracy

![accuracy](https://user-images.githubusercontent.com/69175360/217973058-c90b5b7d-f435-4ef3-b541-6487c552dbe9.JPG)

#### Pie Chart displaying how features were weighted

![download](https://user-images.githubusercontent.com/69175360/221024090-e3388356-a78f-48ed-a841-dd177b700112.png)

#### Pie charts displaying how features were weighed depending on city

![NYVSLA](https://user-images.githubusercontent.com/69175360/221027919-987978d2-8b69-432d-aa9f-393c3787c31c.JPG)


#### Creation of two tables (so far) stored in database

We decided to store our data in a postgres database:

![tables](https://user-images.githubusercontent.com/112716673/217988081-7d084c0c-6135-4d55-b4e6-ec81abea5718.png)

Here is the first table which is our mostly raw data (only url and description taken out):

![image](https://user-images.githubusercontent.com/112716673/217988435-7e98bf27-6a91-4ecb-b58b-5744b584a612.png)

Here is our encoded data from NYC using only 6 features and one output column:

![image](https://user-images.githubusercontent.com/112716673/217988566-fb707ba0-c928-431d-85ff-326675fd6ac5.png)


### Addition of amenities column to our dataset 

In at attempt to better understand what factors influence the price of airBnB listings, we decided to include the amenities column from the dataset. Amenities such as 'Wireless internet', 'Air condiitoning', 'Kitchen', and 'Heating' could all play key factors in the price of the airBnB. While location and number of acommodations remains the primary indicators for how expensive a listing will be, amenities can also play a big role in the price. 

Below is a dataframe and corrosponding bar graph to display the most expensive amenities on average for a rental property in New York City. 

#### Amenities and Availibilities of Features

![amenities and availib](https://user-images.githubusercontent.com/69175360/221025713-7a538d97-ed07-4c57-addd-87ff3cc7c02c.JPG)


### Tableau Visualizations 

Using Tableau, we created several visualizations that would help us display our data and analysis. We created several iterations of heatmaps in various forms to visualize the most expensive locations to rent an Airbnb in New York City based on the same features that we trained the meachine learning model on. 


#### A collection of visualizations created from Tableau

![Airbnb Listings](https://user-images.githubusercontent.com/69175360/221026296-fb4ea213-99a0-480f-b460-93c5938152f3.png)



## results

Currently, our model can predict the log_price of an AirBnB with a Coefficient of Determination of 0.75. This indicates that 75% of the variation in the dependent variable is accounted for by the independent variables in the model. While we are still striving to make changes to our model and improve this value, we feel that this is an acceptable fit for our model. 

Our model has a Mean Squared Error of 0.1121. This value indicates that the model has a better fit to the data, and the predicted values are closer to the actual values. On average, the predicted values of the log_price are off by the square root of 0.1121 from the actual values. We feel that this is an acceptable range for our model to determine the log price effectively. 

Below you can see a visual depicting our model's predictions versus the true values of Log_Price as well as the exact values.

![True value graph](https://user-images.githubusercontent.com/69175360/221025195-e6338c0e-5a5e-49e4-ab92-299950ed6390.JPG)



### Were we able to answer the questions that we seeked to answer at the beginning of the project?

The first question we seeked to answer was “Are certain features more important in some cities versus others?”

The answer is absolutely yes. Features such as room_type remained the most important feature in determining the cost of a rental property in both LA and NYC, however we saw differences in how the number of bedrooms and bathrooms were weighed between the two. Properties in New York City more heavily weighed the zipcode (location) over the number of people that the property could accomodiate. 

We also analyzed the average price of rentals in both NYC and LA based on which specific amentities they had such as "TV", "Pool", or "BBQ".


![NYVSLA](https://user-images.githubusercontent.com/69175360/221029610-2b1c4121-d73f-41c9-bc7f-66bf875716ec.JPG)

![NYVSLAAMEN](https://user-images.githubusercontent.com/69175360/221029608-f3529332-7666-407c-8f9e-c030fe31cd73.JPG)



We also seeked to understand more about which neighborhoods or areas in NYC would be the most or least expensive to rent a property in through Airbnb. We found that Bayside was the most expensive area to rent an Airbnb, while Bay ridge was the least expensive. 

![newyork pic](https://user-images.githubusercontent.com/69175360/221029832-7b6686b6-7f78-48eb-a5b3-ed839dd01e1a.JPG)


We also wanted to learn more about how the average price of an Airbnb changes based on which city it is located. We found that San Francisco was the most expensive city in our dataset on average for an Airbnb rental, with Chicago and New York City being the two lowest. 


![city](https://user-images.githubusercontent.com/69175360/221030139-c841d38e-05e9-418e-b4bb-33db4eaca56c.JPG)

Our fourth and fifth questions were "Which factors influence the cost of an Airbnb the most?" and “What amenities drive up the price of an Airbnb?” which we were able to answer after training our machine learning model on the dataset and identifying which factors were weighed the most when determining log_price. Based on our data, Room_type reigns supreme in determining the cost of an Airbnb. Examples of room types were, "Whole house, single room, etc." The most expensive amentities for Airbnb rentals included "Doorman", "indoor fireplace", and "Cable TV". 

![fetaure importance](https://user-images.githubusercontent.com/69175360/221031003-59383267-4f91-416a-87e4-6335a905db47.JPG)

## Recommendations for Future Analysis

For future analysis, we recommend that the following features or procedures are added

* Feature ranking with recursive feature elimination 

* Natural language processing on reviews & descriptions 

* Inclusion of other cities in the analysis, further comparisons of the amenities and prices based on city. 



