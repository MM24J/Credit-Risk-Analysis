# credit-risk-classification

**Overview of Analysis**

The purpose of this analysis is to assess creditworthiness of borrowers for a peer-to-peer lending service using historical lending activity. The historical data on 75,000+ borrowers consisted of loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and the status of the loan - whether it is healthy or at risk of defaulting. This data can be used to predict the likelihood of default of loans in the future. The first step was to separate the data into features, consisting of the variables being used to predict the loan status, from the loan status itself. This revealed that 75,036 loans were "healthy" whereas 2500 loans were at risk of default. The data was split into training and testing datasets in order to create a model, fit the data, and make predictions. The machine learning technique of Logistic Regression was used since the outcome variable consisted of two categories (0 = healthy, 1 = unhealthy).

**Results**

The model's performance was evaluated using the balanced accuracy score, confusion matrix, and classification report.
* The balanced accuracy score of the model is 0.97, and the f-1 score is 0.99.
* The weighted average of precision and recall scores is 0.99.
* The precision and recall scores of "healthy" (0) loans are 1.00 and 0.99 respectively.
* The precision and recall scores of "unhealthy" (1) loans are 0.84 and 0.94 respectively.

**Summary**

This model is very good at predicting creditworthiness of borrowers. It is nearly perfect in predicting healthy loans. Where it is weaker is in its ability to predict unhealthy borrowers. It's possible that the bank is excluding some people who may be healthy borrowers as the number of "false negatives" is only 36, which means that there were only 36 out of 75,000+ loans not expected to default which would be predicted incorrectly. There is still a relatively small proportion of loans that would be predicted incorrectly to default compared to the true outcome. Using this model would allow the lender to act conservatively in its judgement of borrowers. It would enable them to make healthy loans and be fairly cautious when screening out potentially unhealthy borrowers at the risk of losing some customers who may in fact be creditworthy.


