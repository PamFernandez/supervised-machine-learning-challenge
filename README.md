### supervised-machine-learning-challenge
# Predicting Credit Risk

### This assignment was to build a machine learning model to attempted to predict whether a loan from Lending Club will become high risk or not.
----------------------------
----------------------------

## Process
I was given two files - all of 2019 Lending Club data, and the 2020Q1 Lending Club data. I used the 2019 data to predict the credit risk of loans from the first quarter of 2020. 

I first used pd.get_dummies() to create a training set of all numeric data from the 2019 loans. I then did the same thing to the 2021Q1 data.

I created two models to fit (train) the data - a Logistic Regression Model and a Random Forest Classifier Model - and I printed the scores for each model.

Before I ran these two models I made a prediction that the Random Forest Classifier Model would perform better. I based this prediction off the knowledge that the Random Forsest Classifier Model performs better with categorical data. And I knew that our target data is in two categories - low risk and high risk.

I then used StandardScaler to scale the training and testing sets and I re-ran both models.

Again before I re-ran these two models I made a prediction. This time I predicted that the testing score for the Logistic Regression Model would improve, but the scores for the Random Forest Classifier Model would be unchanged. I based this predition off the knowlege that scaling improves performance for Logistic Regression but Random Forest is not affected by scaling becasue it is a probability based model which means it doesn't have a distance measurement component to scale.

Both of my predictions proved correct. The Random Forest Classifier Model did perform better than the Logistic Regression Model. And the Logistic Regression Model did improve with scaling. I didn't know how much scaling woud improve the Logistic Regression Model, but was a little surprised to see that it improved enough to out perform the Random Forest Classifier Model.

## Code
* VSCode: CreditRiskEvaluator.ipynb

