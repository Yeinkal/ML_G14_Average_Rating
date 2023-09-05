# MLAveragRatingG14
This project is a Book rating predicting Model which enables us to predict the Average rating of one book 
just  by giving  some information.

# Python version

Python  version 3.11.4

Environment This project was coded with anaconda and Jupyter notebook

# Packages used

pandas as pd

numpy as np

matplotlib inline

pyplot as plt

seaborn as sns

datetime, date, time

plotly.express as px

# Data

One file for the data : "books.csv", at the root the directory


# PROJECT DESCRIPTION


## 1 STEPS : CHECK THE DATASET


  After importing the necessary packages for our program we have. We did a global check of our dataset:
    - check the type of each attribute, 
    - search for missing values,
    - check the name of each attribute, 
    - search for the number of unique values ​​of each attribute.

    
## 2 STEPS : GLOBAL ANALYSIS 


  We did an overall analysis of our dataset by checking the different metrics of the numerical value of the dataset on the one hand and the non-numerical value on the other hand.
  

## 3 STEPS: DATA ANALYSIS AND FEATURE SELECTING


  After that we have carefully studied the average rating attribute which will be the value that our model must determine for each book. 
  
  Subsequently we carried out correlation studies between the Average Rating attribute and 4 numerical variables which seemed relevant to us for our training after having analyzed our dataset. these variables were:
  -  num_pages, 
  -  rating count, 
  -  text review count and 
  -  publication data which we transformed into Book_age to make it easier for us to manipulate this attribute.
    
  For each attribute studied in relation to the average rating variable. We at same time removed the values ​​which seemed outlier to us, adjusted the values ​​which seemed to us inconsistent or poorly informed by assigning chosen values ​​which seemed more logical to us or by affecting the average of the variables.


## STEPS : 4 TRAINING THE MODEL


   After all this descriptive and comparative analysis, we decided to use our 4 preselected attributes after processing as training variables.
    For the modeling part, we chose to do modeling based on Linear models. Our approach was a comparative approach of 3 models and the model which is the most precise will be taken as the definitive model: 

  These models was:   
  - Ramdom forest
  - - Decision Tree
    - - Linear regression
      - - We tested the neural network model as a bonus
          


  ## STEPS: 5 EVALUATE MODELS AND COMPARE THEM

  
   To evaluate the performance of our models we decided to use the following metrics:
   
    - MAE : Mean Absolute Error 
    - MSE : Mean Square Error
    - ME  : Max Error 
   
   After evaluating the metrics we concluded that the Ramdom forest and linear regression models had the best performance with a slight advantage for the Ramdom forest models.
   But globaly All three did a fairly great job and we saw that Neural Network model is very very bad to predict this kind of values
