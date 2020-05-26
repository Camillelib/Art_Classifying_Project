# Supervised Machine Learning Project
Classifying a dataset using an optimised ML model with python

<div><img src="https://angeliquepanagos.com//wp-content/uploads//2016/01//Superma-7660041_630x210.jpg" style="width: 4000px;"></div>

## Overview
Using several machine learning models, can we predict the type of a supermarket based on sales data?

## Process followed

### Librairies used
* pandas
* numpy
* matplotlib.pyplot
* seaborn
* sklearn
* xgboost

### Steps
<b>1. Data collection</b>
<p>Dataset imported from : https://www.kaggle.com/devashish0507/big-mart-sales-prediction</p>

![Types](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/1.%20Number%20of%20outlet%20types.png?raw=true)

<b>2. Data cleaning:</b>
 * Deleting 2 columns
 * Deleting ~6000 empty rows  
 * Cleaning the item fat content column
  
<b>3. Data visualisation: </b>
Understanding the dataset and features.

1. General Product Categories

![Products](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/2.%20Products.png?raw=true)

2. Breakdown Per Store Type:
* Item visibility

![Item visibility](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/3.%20Average%20visibility%20per%20outlet%20type.png?raw=true)

* Total sales

![Total Sales](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/4.%20Total%20sales%20per%20outlet%20type.png?raw=true)

![Breakdown](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/4b.%20Breakdown%20of%20sales%20per%20outlet%20type.png?raw=true)

* Other features: location and age - not included in the models

![others](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/5.%20Other%20features%20for%20outlet%20type.png?raw=true)
 
<b> 4. Data transformation </b>

* Identify and correct correlations
* Categorize columns containing text using LabelEncoder
* Standardize numerical columns using BoxCox
* Identify and correct outliers

<b> 5. Model building </b>

* Splitting the dataset 70/30 for testing and training

* Building several models and identifying the best one based on its accuracy score:
![Models](https://github.com/Camillelib/Supervised_Machine_Learning_Project/blob/master/Media/6.%20models%20analysis.png?raw=true)

* Improving the model chosen using RFE:
In the end, we deleted 2 other features and kept item visibility and outlet sales as variables to classify an outlet.

## Results
The best model to classify outlets into 4 types for this dataset would be logistic regression. Overall, the 2 most important features identified are the item visibility and outlet sales. 
