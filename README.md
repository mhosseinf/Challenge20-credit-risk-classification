# Challenge20-credit-risk-classification

## Overview of the Analysis

In this analysis, the goal was to build a machine-learning model to predict the loan status of applicants based on given features. The dataset contains financial information, and the task is to predict whether a loan is "healthy" or "high-risk." The variables included in the analysis were explored, and logistic regression was employed as the machine learning algorithm.

The analysis involved standard machine learning procedures such as data preprocessing, splitting the data into training and testing sets, training the logistic regression model, and evaluating its performance using metrics like accuracy, precision, recall, and the confusion matrix.

## Results

### Logistic Regression Model:

* **Training Data Score:** 99.15%
* **Testing Data Score:** 99.24%
* **Confusion Matrix:**
   [[18679, 80],
   [67, 558]]


Classification Report:
                      precision    recall  f1-score   support

0 (healthy loan)       1.00      1.00      1.00     18759
1 (high-risk loan)     0.87      0.89      0.88       625

accuracy                                   0.99     19384
macro avg              0.94      0.94      0.94     19384
weighted avg           0.99      0.99      0.99     19384



Summary
### 1st method
True Positive (TP): 558 (Actual 'high-risk loan' correctly predicted as 'high-risk loan')
True Negative (TN): 18679 (Actual 'healthy loan' correctly predicted as 'healthy loan')
False Positive (FP): 80 (Actual 'healthy loan' incorrectly predicted as 'high-risk loan')
False Negative (FN): 67 (Actual 'high-risk loan' incorrectly predicted as 'healthy loan')
Summary 1st method:
By employing confusion matrices and comparing the aggregate of predicted values for each class, I can tell that the number of true negatives and true positives (actuals) for each categorical class align and match. Summed by both columns and rows and equal. Consequently, we can deem the model as both accurate and precise

### 2nd method
Precision for 'healthy loan' (class 0): 1.00 (almost 100% of the predicted 'healthy loan' are actually 'healthy loan')

Precision for 'high-risk loan' (class 1): 0.87 (87% of the predicted 'high-risk loan' are actually 'high-risk loan')

Recall for 'healthy loan' (class 0): 1.00 (almost 100% of the actual 'healthy loan' are correctly predicted)

Recall for 'high-risk loan' (class 1): 0.89 (89% of the actual 'high-risk loan' are correctly predicted)

F1-score for 'healthy loan' (class 0): 1.00 (harmonic mean of precision and recall)

F1-score for 'high-risk loan' (class 1): 0.88 (harmonic mean of precision and recall)

Summary 2nd method:
The model performs very well for both classes. It has high precision and recall for 'healthy loan' and 'high-risk loan'. The high F1-scores indicate a good balance between precision and recall. The overall accuracy is also high at 99%. These metrics suggest that the logistic regression model is effective in predicting both classes.
