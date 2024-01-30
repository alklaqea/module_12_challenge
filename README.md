Credit risk analysis report:

The purpose of using different models is to see which model predicts high risk loans better.
Failing to identify high risk loans would be very detrimental to the company.

The data was based on loan size,	interest rate,	borrower income,	debt to income,	number of accounts,	derogatory marks,	total debt,	and loan status.
The variable that we were making predictions on was the loan status. Below is the steps that were taken to go through the proccess.

1) Split the Data into Training and Testing Sets
 reading it into a DataFrame, creating labels and features, checking the balance of the labels, and splitting the data

2)Create a Logistic Regression Model with the Original Data
 Fit a logistic regression model by using the training data
saved the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.
Evaluate the model’s performance

3) Predict a Logistic Regression Model with Resampled Training Data
Instantiated the random oversampler model
Fit the original training data to the random_oversampler model
Instantiated the Logistic Regression model
Fitted the model using the resampled training data
Made a prediction using the testing data
Printed the balanced_accuracy score of the model
Generated a confusion matrix for the model
Printed a classification report for the model

LogisticRegression model with orginal data results:


Balanced accuracy score: 0.9918489475856377
Precision score: Healthy loans: 1    High risk loans: 0.85
Recall score: Healthy loans: 0.99    High risk loans: 0.91

Logistic Regression Model with Resampled Training Data:

Balanced accuracy score: 0.9936781215845847
Precision score: Healthy loans: 1    High risk loans: 0.84
Recall score: Healthy loans: 0.99    High risk loans: 0.99

The logisticRegression model with the original data results is the better model. They both have a high accuracy score but the model with the 
resampled data might be overfitted and thats why it has a recall score of 0.99 for the healthy and high risk loans.

