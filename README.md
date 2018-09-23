# Quartic.ai

## Approach Used
For the given problem, various machine learning algorithm was used.
The training data-set was split into 80-20 percent, 20 being used as test data.
The approach I am proposing is based on the concept of bagging, **Random Forest**, the model constructed shows good results as compared to other techniques.

Other concepts used:
|No| Technique| Analysis|
|-|-|-|
|1| Boosting                   |time consuming while training the model|
|2| Naive Bayes                |accuracy was lower compared to the selected approach|
|3| Logistic Regression        |accuracy was lower compared to the selected approach|

Starting with the process, data analysis was carried out. The data had many missing values, due to the nature of the missing values, two techniques were used to treat the missing values, namely **bfill** and **ffill**.

Further analysis of test data denoted **imbalanced classes**, to resolve the same we over-sampled the minority data using **SMOTE**. This process rectified the imbalanced data-set problem.

After data analysis was complete, model creation was carried out. Then using the accuracy score and confusion matrix the performance of the model was ascertained. The accompanying code has all the measurements.
**Accuracy Score: 98.07%**

## Performance, Complexity & Bottlenecks
The performance of using the selected approach is good as it is 98.07% accurate in predicting values.
||Predicted: No|Predicted: Yes|
|-|-|-|
|**Actual: No**| 115097     | 7|
|**Actual: Yes**| 4419 |110191|

The model is fairly simple and does not have any complexity.

The only bottleneck faced was the presence of imbalanced data-set, the bagging technique could get trained with a bias and thus incorrectly classify. Therefore a balanced and proper data-set is required.

## Improvements
Few improvements which can be checked out:

1) Any other method of over-sampling of data - imbalanced class problem
2) Any other method of missing value treatment
3) Any other method of classification like SVM or changing various factors of boosting.

**[Data Set](https://drive.google.com/drive/folders/1E-2KIgQdYQBk78IWnAgTnNrhC9PE83Qz?usp=sharing)**
