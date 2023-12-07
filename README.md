### Credit Risk Analysis Report

Using the financial data provided in "lending_data.csv" we are building a model that will help assess credit worthiness amongst applications amongst peer to peer lending services. The process will review two different model building techniques (LogisticRegression with provided data and with additional data utilizing the RandomOversampler) to identify which is better at predicting and identifying credit worthiness.

LogisticRegression with standard data model identifies the following:
Overall Performance (avg):
* Balanced Accuracy Score: 95%
* Average Precision Score: 99%
* Average Recall Score: 99%
Healthy Loan Prediction:
* Precision Score: 100%
* Recall Score: 99%
High Risk Loan Prediction:
* Precision Score: 85%
* Recall Score: 91%

LogisticRegression with RandomOversampler data model identifies the following:
Overall Performance (avg):
* Balanced Accuracy Score: 99%
* Average Precision Score: 99%
* Average Recall Score: 99%
Healthy Loan Prediction:
* Precision Score: 100%
* Recall Score: 99%
High Risk Loan Prediction:
* Precision Score: 84%
* Recall Score: 99%

Comparative review of the scores returned from the two models identifies a that there is not much difference between the two models amongst Healthy Loan Prediction. However, when we review the High Risk Loan Predictions, it appears that the over sampled model increases recall by 8% points while only decreasing precision by 1% point. This would imply that the oversampled model yields better results when trying to predict High Risk Loans. In this instance we would likely choose the oversampled model to restrict the number of high risk loans that are issued.