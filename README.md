# P2P-Lending-Credit-Risk-Classifier-with-Machine-Learning

This application compares two methods of machine learning to analyze credit risk. A dataset of historical lending information is used. The two models used both use logistic regression, with one of them applying oversampling of the target data due to its low representation in the original data set. The two models will be compared for their usefulness with the metrics of precision and recall, recall being the percent of high risk loans being correctly identified and precision being the percent of loans the machine flags as being correctly identified.

# Technologies

This program was written in Python 3.7 and can be run in Jupyter Lab.

The following libraries are used:

- pandas
- numpy
- sklearn
- imblearn

# Installation Guide

You will need to verify that you have installed the libraries listed in the Technologies section.

# Usage

The application `credit_risk_resampling.ipynb` can be run in Jupyter Lab. 

## Contributors
This program was written by Preston Hodsman based on a request for analysis from Trilogy Education Services, a 2U, Inc.

## License
MIT

# Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

In analyzing credit risk using machine learning techniques, due to the small amount of high risk loans in a dataset, it is possible for the results of a machine learning model to not deliver the best results in trying to identify high risk loans in another similar dataset. In this analysis, two machine learning techniques will be compared on a historical data set for lending activity from a peer-to-peer lending services company. The goal is to find which model is better for identifying creditworthiness of borrowers with similar datasets.

The two machine learning methods compared will both use logistic regression on randomly split versions of the original data, with training sets and testing sets. The training set will be used to train the machine learning model, and then the model will be applied to the testing set to see how well it performs in terms of percent of correctly identified high risk loans, and percent of incorrectly identified high risk loans. Since the amount of high risk loans is a small portion of the dataset, a second model will be run using an imbalanced learning approach that oversamples the amount of high risk loans, and the results will be compared.

In the original training split data set, there were 75036 good loans, and 2500 high risk loans. The resampled training split dataset oversamples the high risk loans to get a better dataset for this particular machine learning algorithm of Logistic Regression to work on, which instead has 56271 good loans and 56271 high risk loans.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

The two models are compared on three main metrics. Accuracy, precision, and recall. Accuracy is the percent of correct predictions, which includes the target(high risk loans) and the non-targets(low risk loans). Precision is the percent of predictions of the target which are correct, so it is a way to measure the percent of false positives of the model. Recall is the percent of the targets that are accurately identified, so it is a way to measure how many of the targets are missed. There is often a tradeoff between getting a higher amount of targets correctly identified and overidentifying and creating false positives for this kind of data, so the tradeoff must be measured for the particular application.


- Machine Learning Model 1: Logistical Regression with Train-Test Split
  - Description of Model 1 Accuracy, Precision, and Recall scores.



- Machine Learning Model 2: Logistical Regression with Resampled Train-Test Split
  - Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
