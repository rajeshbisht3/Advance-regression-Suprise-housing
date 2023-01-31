# Advance regresssion (Surprise housing )

#Problem Statement 

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.


The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.


The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.

#Business Goal

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.
Also, determine the optimal value of lambda for ridge and lasso regression.


## LASSO Regression mOdel 

![image](https://user-images.githubusercontent.com/84132394/215759181-62d8a02d-b139-42e9-bbaf-86bcd05ee877.png)





## Conclusions
# Good score in Lasso Regressio

Model coefficients are listed in a table along with the corresponding features , for example natural log of SalePrice will change by 0.124911 with unit change in the feature '1stFlrSF' when all the features remain constant. Negative sign in the coefficient signifies negative correlation between the predictor and target variable. All the features are then analyzed, missing data handling, outlier detection, data cleaning are done. Trend of SalePrice is

observed for change in individual features.

New features are extracted, redundant features dropped and categorical features are encoded accordingly.

Then the data in split into train and test data and feature scaling is performed.

Target variable SalePrice is right skewed. Natural log of the same is Normal distributed, hence for model building, natural log of SalePrice is considered.

Creating dummy variables increased the number of features greatly, highly imbalanced columns are dropped.

Top 50 features are selected through RFE and adjusted R-square. 50 features :

Ridge and Lasso Regression Model are built with optimum alpha calculated in GridSearchCV method. Optimum alpha = 9.0 for ridge and 0.0001 for lasso model.

Model evaluation is done with R2 score and Root Mean Square Error.

Lasso Regression is chosen as final model for having slightly better R-square value on test data.

Predicted value of SalePrice is tranformed into its original scale by performing antilog

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->



