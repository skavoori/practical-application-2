# practical-application-2

This application demonstrates the usage of CRISP-DM framework and it's applications to analyze a dataset and address problems the framework helps in address. 

## Overview 

The dataset we analyze is of the Used car data. The Used car data consists of information from over 3 million used cars. The dataset contains information on 426k card to ensure speed of processing. 

## Objective 

- To understand what factors make a car more or less expensive. 
- To provide recommendations to a user car dealership on what consumers value in a used car.


## Approach 
Analysis has been performed on the Used car dataset using python pandas library, seaborn library, matplotlib, numpy and scikit learn libraries. Various data exploration techniques, data cleaning techniques, analysis using regression models have been used to understand, analyse and engineer the features required for modeling of the data. 

## Analysis 
- The dataset has 426880 x 18 columns 
- There are a lot of NaN values in the dataset. 
- Out of 18 columns there are 4 numerical columns and 14 categorical columns. 
- There are total 12 different paint colors 
- There is data from all the states of USA 
- After dropping non-null values there were 34868 entries.
- Various plots have been created after cleaning the data. 
- Correlation plots have been drawn for data with numerical columns to derive the relationship between price and the attributes of the car. 


## Data Preparation 
- Dropped Null Values 
- Removed rows that have price values set to 0 
- Dropped the columns that have no impact on price of the car like IDs VIN numbers etc.. 
- Transformed Non Numerical columns into Numerical Columns 
- Used One Hot Encoding for Paint Color. 


## Observations from Modeling the data 
- There is a high correlation between year, number of cylinders and price. 
- There is an inverse correlation between odometer and price. The more the odometer the less the price. 
- Observations from Box Plots of various Categorical Values
- New and Like New Cars can be priced competitively as they seem to get more value 
- Electric and Diesel cars seems to get more price 
- Automatic Transmission seems to be more popular 
- Clean Title helps. 
- Most popular vehicle is the one with 8 cyclinders
- There are more full sized vehicles that are priced well. They seem to be more popular
- Expensive used cars.


## Next Steps  