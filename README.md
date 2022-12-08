# Churn Prediction using Survival Analysis

The main concern of companies that operate with subscription models is customer retention,
unlike traditional companies that focus on product quality and gaining new customers. 

Analyzing and managing the duration of customer contracts is a rather complex problem,
which concerns more and more companies. The purpose of this project is to explain the
survival analysis models and their application for the analysis and prediction of 
customers' survival time.

Survival analysis is a statistical method used to analyze data where the outcome variable
is the time it takes for an event of interest to occur. 
It is a method commonly used in medical research to study the length of time that a 
patient survives after receiving a treatment or to analyze the time it takes for a
particular condition to develop. 

Survival analysis can also be used in other fields, such as economics, engineering, and
social sciences, to study the time it takes for a product to fail or for a customer 
to churn. 

The goal of survival analysis is to understand the factors that influence the time to 
the event of interest and to make predictions about future events.

The project consists of 3 sections/steps that are explained below

The dataset used is named telco_customer_churn, it is located in the data folder, and it 
was derived from kaggle.

## Sections

### 1) Exploratory Data Analysis (EDA) :mag_right:
**Exploratory data analysis (EDA)** is an essential step in the data analysis process 
because it helps to identify potential issues or anomalies in the data and to develop 
a deeper understanding of the data. In this section I 
* use some basic visualizations to better understand the data 
* and decide how should I do the data 
  cleaning.

### 2) Feature Engineering :wrench:
**Feature engineering** is the process of transforming raw data into features that can be 
used in machine learning and statistical learning algorithms. It is an essential step in 
this process because the quality of the features that are used to train a model can 
have a significant impact on its performance. In this section I 
* re-label some dimension columns by creating dummy variables, 
* turn boolean columns to zeros(0) and ones(1), 
* drop some rows with many NULL values 
* and drop some dummy variables since their info can be derived from other variables.

### 3) Fitting Survival Analysis Methods :bulb:
The most common methods for Survival Analysis is the **Kaplan Meier Curves** and the 
**Cox Proportional Hazards model**

In this section I fit the data in these models and by making some minor tweaks.
The goal of this section is to come up with some visualizations that would help me 
estimate when a customer will churn. 

**BUT**

Knowing only when the customer is expected to churn wouldn't help the company retain 
the customer. The most interesting part of this analysis is that by taking into account 
the features of the aforementioned models along with their weight, the company can now 
understand the reason that each customer is willing to churn!
