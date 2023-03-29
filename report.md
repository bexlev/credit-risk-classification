# Module 12 Report: Credit Risk Classification through Supervised Learning


## Analysis Overview


The purpose of this analysis is to train and evaluate a supervised model's ability to predict loan risk, using a dataset containing historical lending activity. The goal of the model is to identify creditworthiness of borrowers.

In this model, the variable loan_status was used as the label, while the remaining columns were classified as features (loan_size, interest_rate,	borrower_income,	debt_to_income,	num_of_accounts, derogatory_marks, total_debt).

The data was split into training and testing datasets, then fit to a logistic regression model. 
The model's performance was evaluated through an accuracy score, confusion matrix, and classification report. 


## Results: Evaluation of Logistic Regression Model

Accuracy Score : 0.9918489475856377
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384



## Summary

Overall, the model accuracy is very high at 0.99, and the precision and recall are very high as well. However, I would want to continue training, as the precision and recall for 1 is lower than that of 0, and as 1 signifies a high-risk loan, I would want to avoid mistakes there, as this would lead to more loan rejections than necessary. 