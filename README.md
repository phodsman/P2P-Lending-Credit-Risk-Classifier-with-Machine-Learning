# P2P-Lending-Credit-Risk-Classifier-with-Machine-Learning

Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. In this analysis, two machine learning techniques will be compared on a historical data set for lending activity from a peer-to-peer lending services company with the goal of finding which model is better for identifying creditworthiness of borrowers.

The two machine learning methods compared will both use logistical regression on randomly split versions of the original data, with training sets and testing sets. The training set will be used to train the machine learning model, and then the model will be applied to the testing set to see how well it performs in terms of percent of correctly identified high risk loans, and percent of incorrectly identified high risk loans. Since the amount of high risk loans is a small portion of the dataset, a second model will be run using an imbalanced learning approach that oversamples the amount of high risk loans, and the results will be compared.

# Technologies

This program was written in Python 3.7 and can be run in Jupyter Lab.

The following libraries are used:

- pandas
- numpy
- sklearn
- imblearn

# Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
