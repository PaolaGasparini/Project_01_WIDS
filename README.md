# Project 1 Women In Data Science 2021

This is the repo for Project 01. 

This repo contains the source code of the Exploratory Data Analysis for the Kaggle website "Women in Data Science 2021"(https://www.kaggle.com/c/widsdatathon2021)
regarding patients with Diabetes Mellitus in Intensive Care Unit.
In this repository you can find the jupyter notebook wids_workbook.ipynb. The source data can be found from this link (https://www.kaggle.com/c/widsdatathon2021):  TrainingWiDS2021.csv, UnlabeledWiDS2021.csv. 


## Table of Contents

* [Libraries](#Libraries)
* [Questions](#Questions)
* [Results](#Results)
* [Creator](#Creator)
* [Acknowledgement](#Acknowledgements)


## Libraries

To run this notebook the librarie to install are the following. 
* pandas
* numpy
* seaborn
* matplotlib
* fancyimpute
* sklearn
* imblearn


## Questions

In the Jupyter Notebook we are answering the following questions:

 1) What are the variables that are highly correlated with the Diabetes Mellitus (target one)?
 2) What are the ones that have a low correlation with it?
 3) Considering our dataset, which disease is causing more number of days in hospital admission before icu (pre_icu_los_days)?
 4) Considering the correlation between weight and Diabetes Mellitus, is there a significant difference in weights among people with different ethnical backgrounds?
 5) Sometimes in the Intensive Care Unit (ICU) there are patients that don't have a complete clinical history immediately available.  In ICU time is very important to save lives and the question many doctors want to know is the following: can we derive if a patient has the Diabetes Mellitus (chronic disease) from the tests that we are doing when we admit him in the unit?
 

## Results

To answer the questions we are using the typical steps of a data science process: gather, assess, clean, analyze, model and visualize. 
The visualisation of the data is a continous point that is happening during all the steps of the process. 
The conclusions are the following:
1) Some variables like glucose, BMI and weight are highly correlated with diabetes
2) Some variables like the lowest blood pressure noninvasive or lowest hematocrite (volume proportion of red blood cells) are negative correlated with the variable diabetes.
3) There isn't a significant difference in terms of pre Intensive Care Unit length of stay among diseases. When leukemia, lymphoma, aids and solid_tumor_with_metastasis are present we can see that they have a higher variance of this variable compared to the other diseases or a situation without a disease.
4) Asian people have the lowest weight compare to the other ethnicity. In all the ethnicity the weight is higher in people with diabetes compared to the people with no disease but we can see that the biggest difference is in the Caucasian, African American and Native American population.
5) A XGboost is giving good results to predict diabetes mellitus in terms of overall accuracy 0.81 and a good recall for the minority class (1=diabetes mellitus) as well.

A Medium blog on this topic has been created at the following link: https://medium.com/@gaspap87/machine-learning-can-save-lives-99b243de7dba

## Creator

* Paola Gasparini
  [https://github.com/PaolaGasparini](https://github.com/PaolaGasparini)

## Acknowledgements
This notebook was created using the datasets available in the kaggle competition https://www.kaggle.com/c/widsdatathon2021


