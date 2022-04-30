# House_rent_prediction
House Rent prices can be hard to understand due to the lack of information and the complexities of the real estate market. 
Airbnb is a platform for marketing and renting properties for shortterm stays. Airbnb listings contain a lot of information that can help predict the price 
associated with that list. The relationship between Airbnb listing prices and average real estate prices in the vicinity of these listings is explored. 
Multiple Machine Learning algorithms are considered: Linear Regression, Support Vector Machines, K-Nearest Neighbor, Decision Tree, Naive Bayes, and 
Stochastic Gradient Descent.Finally, each of these algorithms are ranked by effectiveness and considered both with and without real estate estimates as features.

From Zillow, we get a dataset containing a time series estimates for the average rent price for
a Single Family Residence for most zip codes in the US. Yet, for this research, we don’t need
an entire time series worth of estimates. Instead, we need a single value per zip code.
In order to get that single value, we consider the upload date of each Airbnb dataset and use
that upload date as the canonical date for all of the listings in that dataset. For each zip code,
we either extract the value at that date or, if missing, consider the closest value to that date. In
full, in order to model the “price” target feature, we consider the following features:
 Property Type (categorical)
 Room Type (categorical)
 Number of Accommodates (continuous)
 Number of Bathrooms (continuous)
 Number of Bedrooms (continuous)
 Number of Beds (continuous)
 Bed Type (categorical)
 Average Rent (continuous)
We believe that the application of machine learning algorithms on these features will yield
improved results.

Furthermore, as regards the ranking of Machine Learning algorithms, we consider multiple
regression metrics:
 Mean Absolute Error
 Mean Squared Error
 R2 Error
