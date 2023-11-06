# Ames Housing Data and Kaggle Challenge

## Problem Statement

The house pricing is increasing every year. Each home buyer has their own characteristics when they are looking for a house. Before the coronavirus pandemic the house pricing was increasing slightly from year to year but after the pandemic the house pricing was increasing faster than normal. The purpose of this project is to create a model using the Ames Housing Dataset and identify which characteristics have an effect on house pricing.

## Background 

Every home buyer will have their own criteria for their house based on their income and living goal. There are some common criteria for home buyers when they are looking for a house. The first criteria is the price followed by location, house condition, square footage, home type, outside space and and other different criterias.([*source*](https://www.forbes.com/advisor/mortgages/real-estate/what-to-look-for-when-buying-a-house/))

The materials to build houses are limited and the number of home buyers are increasing. Those reasons cause house pricing to increase after the pandemic.([*Read this for more information.*](https://www.whitehouse.gov/cea/written-materials/2021/09/09/housing-prices-and-inflation/))

Iowa is one of the first 10 states that have lowest house pricing. Iowa is a state in the Midwest of the United States and Ames is a city of Iowa. Due to the weather condition,some Iowa’s houses may have a basement. The basement is known as a shelter and one of the characteristics buyers look for.([*source*](https://lovehomedesigns.com/where-are-basements-common/#:~:text=On%20average%2C%20in%20the%20United,%2C%20Oklahoma%2C%20Iowa%2C%20Missouri.)). Besides the basement, home buyers are also looking for different characteristics, for example, when the house was built or remodeled. Exploring the Ames Housing dataset to find more characteristics. 

## Dataset 

* [`train.csv`]('../datasets/train.csv'): Ames Housing Dataset
* [`test.csv`]('../datasets/test.csv'): Ames Housing Dataset without sale price

**Brief description of the contents for each dataset.**

The train dataset have 80 columns are criteria of a house and the last column is sale price.
The test dataset have 80 columns are criteria of a house.

Read this for each criteria description. ([data description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt))


## Preprocessing and Modeling 

Apllying linear regression, lasso, and ridgetest to evaluate a variety of models to identify a production algorithm.

## Modeling Interpretation & Conclusions

* Model 1 and model 2 are predicted base on 87 features including some objects features after OneHotEncorder by applying Linear Regression model, Ridge model, and Lasso model. The train score of all the models are little higher than test score. Both models are underfit. To improve the underfit of both models, I should add more features and try some different range of alpha on ridge and lasso model.
* The Root Mean Squared Error (RMSE) of the model 1 and model 2 are high. The values of the RMSE are high may be due to some outliers.
* The RMSE in the Linear Regression model are higher than Ridge and Lasso model. In model 1, the RMSE of Linear Regression is around 28492.93, RMSE of Ridge is around 28237.79, and RMSE of Lasso is around 28050.53. In the model 2, I keep the Linear Regression model the same but change the range of alpha in Ridge and Lasso model. The RMSE of Ridge in model 2 is around 28161.30 and lower than model 1 but the RMSE of Lasso in model 2 is higher than model 1, it is around 28484.64.
* In model 1, the best test score (around 0.872) and the lowest MSE is from Lasso model. In model 2, the best test score (around 0.871) and lowest MSE is from Ridge model.
* In conclusion, model 1 and model 2 cannot be use to predict the sale price due to the high value of MSE. In the future, may be add more features, try some different model and different range of alpha on Ridge and Lasso.

