# Project on Machine Learning and Data Science

## Make Two Project 
 #### 1. Heart-Disease-Project
 #### 2. Predicting The Sale Price of Bulozers (Regression)

 #  1. Heart-Disease Project  (Based on Classification Model )Details
 
## Predicting heart disease using machine learning 

This notebook looks Into Using Various Python-Based Machine Learning and Data  Science libraries in an attempt to build a machine learning model capable of predicting whether or not someone has heart disease based on their medical atrributes.

## we're going to take the following apprach:
1. Problem definition 
2. Data 
3. evalutaion
4. Features
5. Modelling 
6.Experimentation

## 1. Problem definiton

> Given clinical Parameter about a Patient, can we predict whether or not they have heart Disease?
## 2. Data

The Original data came from the cleavland data from the UCI Machine Learning Learning Repository 


There is also a version of its aviable on Kaggle.


## 3. Evaluation 

> If we can reach 95% accracy at predicting whether or not a patient has heart disease during the proof of concept, we'll purse the project .

## 4. Features 

This is where you'll get different information about each of the featurein your data.


**Creating Data Dictionary**


* agage in year 
* sex (1 = male; 0=female)
    *
* cp chest pain type 

    * 0:Typical angina: chest pain related decrease blood supply to the heart 
    * 1: Atypical Angina: chest pain not related to heart 
    * 2: Non-anginal Pain: Typically esophageal spasms (non heart related)
    * 3: Aysmptomatic: chest pain not showing signs of disease 
    
* trstbps- resting blood presure ( in mmHg on admission to the hopital) anything above 130-140 is typically cause for concern


* chol- serum cholestoral in mg/dl

    * serum =LDL+HDL +.2* triglcerides
    * above 200 is cause for concern
    
* fbe(fasting blood sugar >120mg/dl)(1= true;0 =false)
    * \>126mg/dl sing diabetes
* restecg- resting  electrocardiographic result heart rate achieved
    * 0:Nothing to note
    * 1:ST_T wave abnormality
        * can range from mild symtoms to severe problems 
        * signals non-normal heart beat
    * 2: Possible or definite left ventricular hypertrophy
        * Enlarged Heart's Main pumping chamber
        
* thalach- maxium heart rate achieved 
* exangex- ercise include angina(1=yes; 0=no)
* oldpeak- ST depression induced by exercise relative to rest looks at stress of heart stress more
* slope- the slope of the peak exercise ST segment
   
   * 0: Upslping better heart rate with excercise (uncommon>
   * 1:Flatsloping: minimal change (typical healthy heart )
   * 2: Downslopins: signs of unhealth heart 
   
* ca- umber of major vessels (0-3) colored by floursospy
    * colored vessel means the doctor can see the blood passing through
    *  the more blood movement the better (no clots)
    
* thal

    * 3 normal; 
    * 6=fixed defect;used to be dect but ok now
    * 7=reversable defect: no proper blood movement when excercising 
    
* target- have disease or not (1=Yes or 0=No)(= the Predicted attribute)

## 5. Modeling

------------------------------------------------------------------------------------
# 2. #  Structured Data Project 2: predicting the sale price of Buldozers (Regression Model)
# 🚜 Predicting the Sales Price of Bulldozers using Machine Learning 

In This notebook, we're going to go  through an example Machine Learning project with the goal of predicting the sale price of bulldozers.

## 1. Problem Defition 

>Predict the auction sale price for a piece of heavy equipment to create a "blue book" for bulldozers.
> How well can we predict the future sale price of a Bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?


## 2. Data 

The data is downloaded from the kaggle bluebook for Bulldozers competition:
you are predicting the sale price of bulldozers sold at auctions.

There are Three main Datasets:https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

The data for this competition is split into three parts:

   * Train.csv is the training set, which contains data through the end of 2011.
   * Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
   * Test.csv is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.

The key fields are in train.csv are:

    SalesID: the uniue identifier of the sale
    MachineID: the unique identifier of a machine.  A machine can be sold multiple times
    saleprice: what the machine sold for at auction (only provided in train.csv)
    saledate: the date of the sale


## 3. Evaluation 

The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

for more on the evaluation of this project check: https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview/evaluation

**Note:** The Goal for most regression evaluation metrics is to minimize to error. For example, our goal for this project will be to build a   machine learning model which minimises RMSLE.


## 4. Features

Kaggel Provides a data dictionary detailing all of the features of the datasets. You can view this datadictionary on google sheet:https://docs.google.com/spreadsheets/d/18ly-bLR8sbDJLITkWG7ozKm8l3RyieQ2Fpgix-beSYI/edit#gid=1021421956

## 5. Modeling 
Making using RandomForestRegression 
