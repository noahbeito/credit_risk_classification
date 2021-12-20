# Credit Risk Analysis Report

Using the imbalanced-learn library and a logistic regression model to compare two versions of the lending_data dataset. The first model uses the original dataset. The second model uses the RandomOverSampler module from the imbalanced-learn library to resample the data.

For both cases, we get the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

---
## Comparing Linear Regression Models:

### Definitions:
* Balanced Accuracy Score: The average of the recall of both classes which can also be described as the average of the true positive rate and the true negative rate. This metric is especially useful when the two classes are imbalanced. 
* Precision: Also known as the positive predictive value. This metric evaluates the percentage of true positives correctly predicted. This is calculated by dividing the number of true positives by the total number of true and false positives.
* Recall: The percentage of all values in a single class that the model correctly predicted divided by the total number of transactions in that category.
---
### Original Data
* Balanced Accuracy Score: .95
* Precision: This logistic regression model predicts the healthy loan label with nearly 100% precision, however, it only predicts the high-risk loan label with 85% precision.
* Recall: The model predicted about 1% of actually healthy loans as risky. The model does not perform quite as well when predicting high risk loans. The model predicts high-risk loans correcly about 91% of the time. The model incorrectly predicted 56 high risk loans as healthy loans.
![image](https://user-images.githubusercontent.com/90667844/146705008-f657d543-d26f-4e87-adb4-c7d30f0e773d.png)
---
### Oversampled Data
* Balanced Accuracy Score: .99
* Precision: This oversampled data model also predicts the healthy loans with a very high precision, still just under 100%. It predicts the high-risk label with about 84% precision, only slightly worse than the original data model. 
* Recall: This model predicted 99% of the high risk loans correctly, only incorrectly predicting 4 as healthy loans
![image](https://user-images.githubusercontent.com/90667844/146704896-bcce6d16-869e-4da4-ae9a-b44f3284ff2a.png)

---
## Summary 
The model fit with the oversampled data has a higher balanced accuracy score, meaning it does a better job at detecting true positives and true negatives. The higher recall in the oversamped data model means that this model correctly predicted a higher percentage of the truly high-risk loans. The oversampled data model is overall much better at predicting high-risk loans. For the purposes of loan qualification, I recommend the Oversampled Data Model, because it does a much better job of predicting the high-risk loans, while still maintaining a high precision predicting healthy loans. 
