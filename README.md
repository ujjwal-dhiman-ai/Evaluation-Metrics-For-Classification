# Evaluation-Metrics-For-Classification

## 1. Confusion Matrix

A confusion matrix is a n * n matrix, where n represent the number of classes in the target variable. There can be multiple classes in the dependent variable.

!(https://github.com/ujjwal-dhiman-ai/Evaluation-Metrics-For-Classification/blob/main/Screenshot%20(123).png)

## 2. Accuracy 

It is the ratio of correct predicted values over the total predicted values.

Accuracy = Correct Predictions / Total Predictions

## 3. Precision and Recall

**Precision:** It is defined as the ratio of the values predicted as positive that were actually positive, over total predicted positives.

Precision = Predictions Actually Positive / Total Predicted Positive

**Recall:** Out of all actual positive, how many are predicted positive

Recall = Predictions Actually Positive / Total Actual Positive

## 4. The ROC Curve

The recevier operating characteristics (ROC) curve is very similar to the precision/recall curve, but instead of plotting precision vs recall, the ROC curve plots the true positive rate(recall) against the false positive rate.

False Positive Rate (FPR) = 1 - True Negative Rate(TNR), where TNR is specificity.

Hence ROC plots sensitivity(recall) versus 1 - specificity

We can compare two classifiers by measuring the area under the curve(AUC). Classifier with higher AUC is considered as best.
Perfect Classifier has ROC AUC = 1
Purely Random Classifier has ROC AUC = 0.5

You should prefer the PR curve whenever the positive class is rare or when you care more about false positive than false negative, and the ROC curve otherwise.
