# Module_12_Challenge
Credit Risk Analysis using Logistic Regression Models and Oversampling.

## Overview of the Analysis

* The purpose of the analysis is to build a model that can identify the creditworthiness of borrowers.
* The model will use a dataset of historical lending activity from a peer-to-peer lending services company.
* The data is imbalanced, with 75036 "healthy loans" and 2500 "high-risk loans".
* The stages of the machine learning process I completed as part of this analysis:
  * Split the data into training and testing datasets
  * Create a Logistic Regression Model
  * Make a prediction using the testing data
  * Generate a balanced accuracy score, a confusion matrix, and a classification report
* Since the data was imbalanced, I used the random oversampling method and built a Logistic Regression Model fit with the oversampled data to compare to the model fit with original data.

## Results

* Machine Learning Model 1: Original Data
  * ![image](https://github.com/tjohnce55/Module_12_Challenge/assets/144564878/70019a57-a7d0-447c-99ce-bdb20f9c407c)
  * The Logistic Regression model does extremely well at predicting 'healthy loans' with precision and recall at 99% and 100%. It is worse at identifying 'high-risk loans', with a precision of 91% and a recall of 85%. Overall the logistic regression model has an average precision and recall of 99%, and a balanced accuracy score of 95.2%.



* Machine Learning Model 2: Oversampled Data
  * ![image](https://github.com/tjohnce55/Module_12_Challenge/assets/144564878/f8cb0410-0302-4847-9b22-cdb2174aa4e2)
  * The accuracy score for the ligistic regression model fit with oversampled data is 99.3%, which is higher than the model with imbalanced data (95.2%). The recall for the high-risk loans increased significantly when the model was fit with oversampled data, increasing from 85% to 99%, while the precision for high-risk loans dropped a bit from 91% to 84%. The precision and recall for healthy loans remained nearly perfect.

## Summary/Conclusion

Based on the results, the machine learning model fit with the oversampled data seems to perform best. Recall is important in this situation because it would be very undesirable for the lending company to identify a 'high-risk loan' as a 'healthy loan' and lend out funds to that 'high-risk' borrower, which will likely lead to loss of funds for the lending company. The second model we analyzed, fit with oversampled data, had higher recall than the model fit with orignal (imbalanced) data. I would definitely recommend thast the lending company use the Machine Learning Model 2 that used the random oversampling method.
