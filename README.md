# Surprise-Housing Prediction
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.The company is looking at prospective properties to buy to enter the market.


## Table of Contents
* [Business Overview](#Business-Objective)
* [Technologies Used](#Technologies-Used)
* [Exploratory Data Analysis & Model Steps](#Steps)
* [Conclusions](#Conclusions)

## Business-Objective

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.The company is looking at prospective properties to buy to enter the market.

-  This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.

- The company wants to know:

- - Which variables are significant in predicting the price of a house.

- - How well those variables describe the price of a house.

> dataset : train.csv

## Technologies-Used
- pandas      - Version : 1.2.4
- numpy       - Version : 1.20.1
- seaborn     - Version : 0.11.1
- matplotlib  - Version : 3.3.4
- statsmodels - Version : 0.12.2
- pandasql    - Version : 0.7.3
- sklearn     - Version :0.24.2

# Exploratory Data Analysis & Model Steps

## Steps

> ## EDA

- Data Clearning and Missing Data Analysis
- Outlier Analysis & Treatment Assumption values > Q3+1.5*IQR and values < Q1-1.5*IQR will be treated
- Deriving Categorical Columns
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis

> ## ModelPreparation

- Training and Test data split
- Feature Scaling - StandardScaler
- Feature Engineering & Selection using RFE and Variance Inflation factor
- Model preperation using OLS & Linear Regression
- Regularization Ridge & Lasso Regression Model
- Residual Analysis
- Model Evaluation & Assessment
- Prediction
- Final Conclusion & Analysis

## Conclusions


###  EDA ANALYSIS

- YearbuiltAge,YearRemodel_Age and garageYRBT_Age have negative correlation
- House with execellent Kitchenquality & HeatingQC have HighestSaleprice
- House with BuildtinGarageType and Finishes Garage Work have highest SalePrice
- We can observe high no of SalePrice for MSSubClass 80 and then 120
- MSZoning Floating Village Residential have highesst no of SalePrice
- Houses with Excellent ExternalQuality Excellent have highest SalePrice
- Houses with Excellent BasementQuality have highest SalePrice
- With the increase in overallcond SalePrice will increase
- Houses with RoofStyle hip have highest no of SalePrice
- Houses with External Centralboard have highest sale price following BrkFace
- Houses with 2Story and 1Story buildings have highes no of SalePrice
- with the increase in overallquality saleprice will increase
- Neighborhood_Nridght have highest SalePrice
- Building type townhouseend unit and Single Family Detached have highest no of SalePrice

### Model Selection

- All the models are showing almost close R2_score but can see the model R2_Score for lasso regresion is slightly better so we will go with it.

### Significant Variables

GrLivArea 
GarageCars
GarageArea
TotalBsmtSF
OverallQual
Exterior1st
Neighbourhood
MSZoning

## Contact
Created by [@shashank1989] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
