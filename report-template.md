# Module 20 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the analysis was to determine if a LogisticRegression machine would accurately predict healthy loans vs. high risk-loans using the data set provided. The data set included 77,536 loans, including a column on loan status which was used to predict our analysis.


* Explain what financial information the data was on, and what you needed to predict.

The data set included the following columns: loan_size, interest_rate, borrower_income , debt_to_income ratio, number _of_accounts, derotatory_marks, total_debt and loan_status. Loan_status was used in the model for the predictions.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The value_counts were 0 for a healthy loan and a 1 for a high risk loan. This is what we were trying to predict.

* Describe the stages of the machine learning process you went through as part of this analysis.
-Started the process with the import of the csv file, then created the data frame and identified the columns.
-seperate the data into features and labels, the lables were the the loan_status either 0 or 1 and the remaining data is the features that we used to train the model.
- used train_test_split
-imported LogisticRegression from sklearn
- fit the model using the training data and then used the test data to make predictions.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

I used: LogisticRegression from SKlearan, train_test_split from SKlearn, confusion_matrix and classification_report from SKLearn.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  Accuracy: 99%
  precision: 
  0: 100%
  1: 84%
  recall: 
  0: 99%
  1: 94%


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  Accuracy: 99%
  precision: 
  0: 100%
  1: 84%
  recall: 
  0: 99%
  1: 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Both models have  99% accuracy, but  the second model has a higher recall for "1" at 99% compared to 94% from the first Model. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
It is more important to predict the high risk loans "1" than the healthy loans "0". 

Overall the second model outperforms the first model slightly in the "1" recall value and therefore is the better choice. The second model outperforms the first in being able to correctly identify the actual amount of "1" values. The difference of the model could be exxplained by the second model being more balanced.


