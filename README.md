# Practical Application 2

This application demonstrates the usage of CRISP-DM framework and it's applications to analyze a dataset and address problems the framework helps in address. 

## Overview 

### CRISP-DM Framework

<center>
    <img src = images/crisp.png width = 50%/>
</center>

CRISP-DM stands for Cross Industry Specification for Data Mining. It provides a framework for understanding data, preapring data, modeling the data, evaluating the data and deploying the results from the analysis and modeling. The various stages of this process are intertwined and aroun 70% of the time in this process is spent in the data understanding and preparation phase. Some of these phases are repeated multiple times depending on the uresults from modeling and evaluation. 

The dataset we analyze is of the used car data. The used car data consists of information from over 3 million used cars. The dataset contains information on 426k cars to ensure speed of processing. The dataset is available [here](data/vehicles.csv). This dataset was analyzed in Jupiter Notebook prompt [here](prompt_II.ipynb)

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

### General Learnings from data modeling.  

- Modeling large amount of data using Regression Models with Polynomial degree greater than 10 with a column count of more than 10 takes humongous amount of time. 
- Feature Engineering takes multiple iterations to arrive at the best possible features needed for reducing the error during predictions. 
- Data selection and preparation is a very important stage of the whole analysis and would significantly impact the outcome. 

## Next Steps  

### Recommendation for Used Car Dealership 

- Dealers should focus more on EVs as they seem to be pretty popular. 
- Focus more on new and like new cars 
- Lower odometer value helps in obtaining maximum value from price. 
- Automatic Transmission and Clean title are more popular. 
- Among vehicle types, a car with 8 cylinder in more popular.
