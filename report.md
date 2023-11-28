## Overview of the Analysis

The objective of this project is to construct a model aimed at assessing the creditworthiness of borrowers and identifying high-risk loans through the training and fitting of data into different models using logistic regression. The data utilized for model training includes the loan status of each lending request, with various variables such as interest rate, loan size, borrower income, etc.; being analyzed to predict a borrower's creditworthiness. The training data includes labels indicating whether each loan is classified as healthy or high-risk. Two logistic regression models were developed for this analysis; the first model was trained on a segmented subset of the data, while the other on a subset with balanced classes achieved through resampling. Subsequently, both models underwent evaluation using sets of test data, and their performances were assessed using a confusion matrix and classification report.

## Results

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.94427
  * Healthy Loan Precision: 1.00
  * Healthy Loan Recall: 1.00
  * High Risk Loan Precision: 0.87
  * High Risk Loan Recall: 0.89

* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.996
  * Healthy Loan Precision: 1.00
  * Healthy Loan Recall: 1.00
  * High Risk Loan Precision: 0.87
  * High Risk Loan Recall: 1.00

## Summary

With an overall high accuarcy rate for the model, it demonstrates perfect precision when predicting healthy loans with a rate of 1.0. However, for loans flagged as high-risk, the model only has a precision rate of 0.87, thus indicating that these loans were correctly categorized 87% percent of the time. That said, based on our tolerance for losses and the average cost associated with a defaulted loan, the model may become impractical due to excessively high recall and precision values.

The model continues to display perfect precision when predicting healthy loans. For high-risk loans, the precision rate remainns at 0.87, predicting successfully only 87% of high-risk loans. However, this second model had a precision rate of 1.00 for recall, which is an improvement from the first model, thus decreasong the chance that a high-risk loan will be missed. 

For the specific goal of accurately flagging all high-risk Loans, the second model proves strongly favored and may be appropriate for industry applications. Model 2 is going to provide a greater incentive for industry application and will potentially mitigate risk. 
