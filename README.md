# PricePrediction
> Here, i've build a real estate price prediction project which predicts a house price in Banglore.

### OVERVIEW of PROJECT
>This Data Science project strolls through bit by bit course of how to assemble a land value expectation site.We will first build a model using sklearn and linear regression using banglore home prices dataset from kaggle.com. During model building we will cover almost all data science concepts such as data load and cleaning, outlier detection and removal, feature engineering, dimensionality reduction, gridsearchcv for hyperparameter tunning, k fold cross validation etc. 

###Technology and tools wise this project covers:###
1. Python
2. Numpy and Pandas for data cleaning
3. Matplotlib for data visualization
4. Sklearn for model building
5. Jupyter notebook

###Code and Resources Used:###
- **Python Version:** 3.8
- **Packages:** pandas, numpy, sklearn, matplotlib, seaborn
- **Dataset:** [https://github.com/PrachiPatel15/PricePrediction/blob/main/House_prices.csv]

###Data CLeaning###
>After getting the data, I needed to clean it up so that it can be usable for our model. I made the following changes and created the following variables:
- Dropped some of the rows which contained null values
- Added median/mode values to null columns if neccesary

###Feature Engineering###
>Added some feature for better visualisation
>Explored some of the important features and cleaned them up
>Adding and deleting attributes

###Dimensionality Reduction###
>We had some excessive amount of data which can lead our model to predict wrong prices so had to reduced by Dimensionality Reduction
In this, any 'location' having less than 10 data points should be tagged as "other" location. This way number of categories can be reduced by huge amount.

###Outlier Removal###
>!Here we've used some bussiness logic to remove the outliers. What we've done is shown in the below images:[https://github.com/PrachiPatel15/PricePrediction/blob/main/Rajaji_Nagar(outlier).png]
By using some bussiness logic we can have the idea of how we can remove the outliers

###Model Building###
> I've imported LinearRegressing from sklearn to predict the future prices

###Model Performance###
> Next, i've used  K Fold cross validation to measure accuracy of our LinearRegression model and on average model got **80%** accuracy in predicting prices

###Further###
- In the project continuation further what can be added is we can use GridSearchCV for better performance and it will show can we can optimize the output
- After doing that we can build Flask API endpoint and the API endpoint takes in a request with a list of values from a trained data and returns an estimated price.
