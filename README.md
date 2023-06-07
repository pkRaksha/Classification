# Classification
## Project Summary :
The Project is a Classification project, the data set used here is related to a marketing campaign of a Portuguese Bank. The Insights of the data are gained by performing EDA. Before EDA , the data is cleaned , all the null values and Duplicate values are dealt. Essential Visualisations are done to understand the data and gain insights to answer certain questions. Multicollinearity and VIF are performed to understand the correlation of the data.

Before Implementing the classification models, data was supposed to be balanced. SMOTE is used to balance the data and then the classification models are used to fit our data and make predictions.

Following models have been used for predictions:-

Logistic Regression Classifier
Decision Tree Classifier
Random Forest Classifier
K-Nearest Neighbors Classifier
Naive Bayes Classifier
Support Vector Machine Classifier
LGBM Classifier


## Problem Statement
The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. The classification goal is to predict if the client will subscribe a term deposit (variable y).

## Data Variables
Bank Client data:
age (numeric)
job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
default: has credit in default? (categorical: 'no','yes','unknown')
housing: has housing loan? (categorical: 'no','yes','unknown')
loan: has personal loan? (categorical: 'no','yes','unknown')
Related with the last contact of the current campaign:
contact: contact communication type (categorical: 'cellular','telephone')
month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
Other attributes:
campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
previous: number of contacts performed before this campaign and for this client (numeric)
poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
Output variable (desired target):
y - has the client subscribed a term deposit? (binary: 'yes','no')

## Conclusions
The 2nd quarter of the year has the highest number of subscriptions & Month of May has the maximum subscriptions.
Blue-collar, management and technician showed maximum interest in subscription.
Compared to married and single, Divorced people have less interest in term deposits.
People with secondary education followed by tertiary education were subscribed to term deposit.
Generally people who don't have credit in default are interested in a deposit. Majority of the people have a home loan but only few of them opted for a term deposit.
Cellular communication is seen as more effective in comparison to other communication types.
The calls with large duration have more tendency for conversion. Majority of people were not contacted previously before this campaign.
We can choose "KNN" or "Decision Tree" to predict Effectiveness as both of them are showing same accuracy of 88% & F1- Score of (0.8824).
