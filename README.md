# credit-risk-classification
Challenge 20

## Files
  - [Jupiter notebook](Credit_Risk/credit_risk_classification.ipynb)
  - [csv](Credit_Risk/Resources/lending_data.csv)

## Overview of the Analysis

* Purpose of the analysis: Create a model that is predicting the loan risk (0 - healthly loan and 1 - high-risk loan).
* Stages of the machine learning process:
    * Machine Learning Model 1 (Original Data):
        - Preparing Data: Read csv, Create labels and features, split data into training and testing datasets.
        - Machine Learning: Instantiate the Logistic Regression model, fit the model and make a prediction.
        - Evaluate model: calculate accuracy score, generate confusion matrix and print a classification report.
     
    * Machine Learning Model 2: (Resampled Training Data):
        - Preparing Data: Read csv, Create labels and features, initiade RandomOverSampler model, fit original training data to new model.
        - Machine Learning: Instantiate the Logistic Regression model, fit the model and make a prediction.
        - Evaluate model: calculate accuracy score, generate confusion matrix and print a classification report. 

## Results

* Machine Learning Model 1:
  
  * The Logistic Regression Model with Original Data gives 95.2% accuracy score. From classification report we can see that our model is performing well in precision healthy loans and 85% high-risk loans are correct.
In Recall 99% of healthy loans and 91% of high-risk loans are predicted correctly.

* Machine Learning Model 2:
  * The Logistic Regression Model with Oversampled Data gives 99.4% accuracy score. From classification report we can see that our model is performing well in precision healthy loans and 84% high-risk loans are correct. In Recall 99% of healthy loans and 99% of high-risk loans are predicted correctly. 

## Summary

Based on analysis above, Model 2 is performing better than Model 1, as it has better accuracy score, but it gives less accuracy in high_risk precision loans (false negative). 

Overall, I would recommend to use Model 2, because it's more accurate and chance to identify high-risk loan is higher.
