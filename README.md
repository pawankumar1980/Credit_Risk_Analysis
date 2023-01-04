# Credit_Risk_Analysis

## Overview

This analysis aims to predict credit risk using data from LendingClub, a peer-to-peer lending company. We will use supervised machine learning techniques to train and evaluate the data, which has an unbalanced classification problem with more good loans than risky loans. To improve the accuracy of our predictions, we will employ various machine learning algorithms to resample the data and balance the classifications.

## Results

The results for the six machine learning models, including their respective balanced accuracy, precision, and recall scores, are as follows:

### Naive Random Oversampling

<img width="1000" alt="Screen Shot 2023-01-04 at 15 36 33" src="https://user-images.githubusercontent.com/111800568/210645802-cb399456-a52d-4d6e-bde5-5182be5768b7.png">

1. Balanced accuracy score: 64.5%
2. The "High Risk" applications precision rate is only 1% with the recall at 61% giving this model an F1 score of 2%.
3. Precision: The precision is low for High-risk loans and is high for Low-risk loans.

### Smote Oversampling

<img width="1075" alt="Screen Shot 2023-01-04 at 15 43 32" src="https://user-images.githubusercontent.com/111800568/210646378-dc07ee19-fb4e-48f4-8f90-6be76d8f9498.png">

1. Balanced accuracy score reduced to 62.4%.
2. The high risk loans  precision, recall and F1 score is similar to earlier model.
3. Low Risk loans had a precision rate of 100% and a reduced recall rate of 64%.

### Undersampling

<img width="989" alt="Screen Shot 2023-01-04 at 15 45 00" src="https://user-images.githubusercontent.com/111800568/210646587-3ea461d6-879a-4b6d-b3c9-83e94a37ba5c.png">

1. Balanced accuracy score reduced to 51% compared to oversampling models.
2. The High Risk applications precision rate again was only at 1% with the recall at 57% giving this model an F1 score of 1%.
3. Low Risk applications had a precision rate of 100% and with a lower recall at 45%.

### Comibination Sampling

<img width="1014" alt="Screen Shot 2023-01-04 at 15 46 09" src="https://user-images.githubusercontent.com/111800568/210646782-f7d50724-d11d-42c4-9816-2141738e0472.png">

1. The balanced accuracy score improved to 64% when using a combined sampling model.
2. The High Risk applications precision rate again at 1% with recall improving to 70% giving this model an F1 score of 2%.
3. Low Risk applications had a precision rate of 100% and with a hiherg recall at 58%.


### Balanced Random Forest Classifier

<img width="972" alt="Screen Shot 2023-01-04 at 15 51 20" src="https://user-images.githubusercontent.com/111800568/210647739-b6a87c75-ddf1-4ffb-a483-042ead6f97a1.png">

1. The balanced accuracy score increased to 78.8% for this model
2. The High Risk applications precision rate increased to 4% with the recall at 67% giving this model an F1 score of 7%.
3. Low Risk applications still had a precision rate of 100% with a higher recall of 91%
4. The top feature by importance was "total_rec_prncp" at 7.4% of the total.

### Easy Ensemble AdaBoost Classifier

<img width="911" alt="Screen Shot 2023-01-04 at 15 53 20" src="https://user-images.githubusercontent.com/111800568/210647975-a8e289af-fba6-4771-bab6-8b55c09fb85c.png">

1. The balanced accuracy score increased to 92.5% with this model.
2. The High Risk applications precision rate increased to 7% with the recall at 91% giving this model an F1 score of 14%.
3. Low Risk applications still had a precision rate of 100% with a higher recall of 94%.


## Summary

After reviewing all the models, the Easy Ensemble Classifer model yielded the best results, with a balanced accuracy rate of 92.5% and a 7% precision rate when predicting High-Risk applications. The sensitivity rate/recall was also the highest at 91% compared to the other models. The result for predicting Low-Risk applications was also the highest, with a recall  of 94% and an F1 score of 97%. 
