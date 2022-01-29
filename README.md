# SyriaTel Customer Churn ML Predictive Analysis




## Overview

Syriatel is telecommunications company that has concerns regarding churn rate. Using the dataset provided, features shall be investigated to determine if there are predictable patterns that are related to our concern.

## The Problem

This dataset shows that there is a ~14.5% customer churn rate. An decent churn rate is 5-7% annually. This means we have some work to do.

## The Solution
This shall require classification machine learning models to identify what features contribute to the `churn` rate.

Providing a quality service and customer service is part of supporting a company's mission statement. Client retention is a factor that may lead to a consistent, predictable profit if referralls and other profit sources are not included. To stay relevant compared to your competitors, it's important to up to date to your company's data so you can calculate what contributes to a successful quarter and/or year and conduct research how to be ahead of your competitor.

Here are 2 main questions the classification machine learning (ML) models may be able to answer:
- What is the relationship between churn and other features?
- Which features increase the likelihood of churn?

## Data Understanding

The dataset explored features including:
**Categorical data:**
- `true` or `false` 
- `yes` or `no`
**Numeric information:**
- Sum of minutes used (day/eve/night)
- Total charge (day/eve/night)
- Number of voicemails
- Account length
**State information** 

*Throughout the project, we aimed to minimize the **false negative** for our goal of discovering churn.* 
- A **false negative (Type II Error)** means our model is predicting that the customer is not going to cancel when they really are. 

*Our priority is given to the metric of **recall** which were in classification report evaluating the performance of the models.*

*Certain features were not included in this project such as:
- `'total_day_charge'`, `'total_eve_charge'`, `'total_night_charge'`, `'phone_number'`. `'area_codex'`

## Modeling

This project included the use of 5 machine learning models including:
- Logistic Regression
- K-Nearest Neighbors
- Decision Tree Classifier
- Random Forest Classifier 
- XG Boost Model

## Evaluation

**Our XGBoost model performed best compared to 4 other models ran.  
- recall : **~79%** 
- Validation accuracy: **~96%**
**

**All columns with numeric values showed to have the most impact on churn rate.**

**Numeric information:
- Sum of minutes used (day/eve/night)
- Total charge (day/eve/night)
- Number of voicemails
- Account length


## Recommendations

- Create dataset per **state** to allow data analyst to see what he/she can do to improve churn per state.
- Explore the impact of **monthly/annual charge for minutes used & the total monthly/annual charge**. This may be useful to find an **optimal charge per minute** compared to competitors prices to see if this decreases churn rate.


## Files and Folders 

.
├── README
├── Customer Churn .ipynb
│   ├── data.csv
|   |-  Intial_Heatmap.png
|   |-  Second_Heatmap.png   
|    
├── SyriaTel Customer Churn ML Predictive Analysis .pdf
