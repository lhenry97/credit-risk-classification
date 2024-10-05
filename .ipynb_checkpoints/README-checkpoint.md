# credit-risk-classification

## Overview of the Analysis


* The purpose of this analysis is to train and evaluate a model based on loan risk. The data used for this was the lending_data.csv file which contains data points on a borrowers loan size, interest rate, income, debt to income, number of accounts they have, number of derogatory marks, total debt and their loan status. The models aim was to attempt to predict the loan status variable being either 0 (healthy loan) or 1 (high-risk loan). The stages of machine learning process was to first split the data into X and y with X containing the features of the data and y containing the loan_status labels of the data. The data is then split into x and y training and testing datasets using the train_test_split function. As the data being used to train the model is a binary classification (or categorical data) logistic regression was selected to train and fit the model using training data. The testing data was then used to make predictions. A confusion matrix and classification report was then generated to assess the ability of the model to make correct predictions.

## Results

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

        * Accuracy Score: 0.99 or 99%
        * Precision Score:
            * for class 0: 1.00 or 100%
            * for class 1: 0.84 or 84%
        * Recall Score:
            * for class 0: 0.99 or 99%
            * for class 1: 0.94 or 94%


## Summary

The model has a high accruacy (99%) and performs fairly well across both classes. Class 0 (healthy loan) performs exceptionally well with 100% precision and f1-score indicating that it correcly identifies the negative cases with very few false positives. In comparison, class 1 (high-risk loan) showed a precision, recall and f1-score of 84%, 94% and 89% respectively. This indicates that while it was able to correcly identify most positive cases, there is in an increased percentage of false negatives compared to class 0. From this it can be concluded that class 0 performs better than class 1.
Performance does depend on the problem trying to be solved. As the data analysed looks at credit risk, it is more important to a bank to be able to accurately detect whether a high-risk loan is occuring or not. This allows the bank to make the decision of whether they are willing to risk approving a loan or not. 
As this model has a high accuracy, high precision in class 0 and fairly high precision in class 1, it can be recommended as a method for machine learning. It may be worth exploring in future though other non-linear machine learning models like decision trees or random forest to see if precision in class 1 can be increased. 
