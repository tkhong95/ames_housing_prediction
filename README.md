# Project 2 - Ames Housing Data and Kaggle Challenge

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

## Conclusions

* A newer house would have a higher price. 
* The quality of overall material and  finish of the house  go up, the sale price go up. 
* The total square feet of the basement area , ground living area,  and first floor square feet increase the sale price increase.
* Basement  have the height above 80 inches would have higher price than others. 
* Single family house are  popular and have higher pricing. 
* Total rooms of house (does not include bathrooms)  between 7 and 12 would have higher price than others.
