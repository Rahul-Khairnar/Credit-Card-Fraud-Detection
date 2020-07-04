## Credit Card Transaction Fraud Detection - Project Overview

Cyber frauds are increasing day by day in the world. More and more people are looted these days online due to increase in transactions happening via cards and online wallets. Hence
it becomes important to increase the security and stop the online scamsters from looting the masses. Hence, keeping this issue in mind, I have developed a model wherein I have trained it
to detect whether a transaction that has been carried out by a credit card fraudulent or not. The model has an efficiency of about 98% with Logistic Regression.

## About the dataset
* The dataset comprised of both fraudulent and non-fraudulent transactions with 99% transactions lying in non fraudulent transactions.
* The transactions were evenly spread in all levels i.e from as low as $2 to as high as $400.
* The dataset had details of about 2 lakh transactions.

## Processes Involved in the whole Project
* Importing the dataset as a csv and converting it into a dataframe so as to work with pandas on it.
* Exploratory Data Analysis(EDA) to understand the data. Some important insights were gathered from this data exploration, which involved:
    * Number of transactions with NA values.
    * Number of fraudulent transactions and number of non fraudulent transactions.
    * Correlations between the various columns of the dataset.
* Data Visualization to further understand the variations in dataset.
* Data cleaning. This was done majorly to remove the outliers for a more accurate prediction.
* Data sampling. This was done to increase the number of fraudulent transactions so that the model is trained to identify not just the non fraudulent once and not be biased. Various
sampling algorithms were used here which included:
    * Random UP Sampler
    * Random DOWN Sampler
    * SMOTE
    * Near - Miss
* Model Training. Data obtained from all the sampling techniques was fit into four different models to check which performs better.

![alt text](https://github.com/Rahul-Khairnar/Credit-Card-Fraud-Detection/blob/master/Photos/1.PNG "Number of Frauds and Non Frauds")

![alt text](https://github.com/Rahul-Khairnar/Credit-Card-Fraud-Detection/blob/master/Photos/Corr.PNG "Correlations between various values of the dataset")

![alt text](https://github.com/Rahul-Khairnar/Credit-Card-Fraud-Detection/blob/master/Photos/time.PNG "Correlations between various values of the dataset")



## Training a model

* Four different models were used for this project. The models were:
    * Logistic Regression
    * Random Forests
    * XG - Boost
    * K-Nearest Neighbours
* The data obtained from various sampling methods was fit into these models simultaneously and the area under the curve(AUC) was calculated for each one of them. 

## Model Performance

The best performing model was Logistic Regression with the highest area under the curve. The performances for the various models are as follows:
* Logistic Regression: 0.98
* Random Forests: 0.97
* K-Nearest Neighbours: 0.93
* XG-Boost: 0.97


![alt text](https://github.com/Rahul-Khairnar/Credit-Card-Fraud-Detection/blob/master/Photos/auc1.PNG "Correlations between various values of the dataset")

![alt text](https://github.com/Rahul-Khairnar/Credit-Card-Fraud-Detection/blob/master/Photos/auc2.PNG "Correlations between various values of the dataset")

Hence from the above results we can say that logistic regression performs the best and hence can be used for productionization.
 
