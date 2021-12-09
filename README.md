# P2P-Lending-Credit-Risk-Classifier-with-Machine-Learning

This application compares two methods of machine learning to analyze credit risk. A dataset of historical lending information is used. The two models used both use logistic regression, with one of them applying oversampling of the target data due to its low representation in the original data set. The two models will be compared for their usefulness with the metrics of precision and recall, recall being the percent of high risk loans being correctly identified and precision being the percent of loans the machine flags as being correctly identified.

## Technologies

This program was written in Python 3.7 and can be run in Jupyter Lab.

The following libraries are used:

- pandas
- numpy
- sklearn
- imblearn

## Installation Guide

You will need to verify that you have installed the libraries listed in the Technologies section.

## Usage

The application `credit_risk_resampling.ipynb` can be run in Jupyter Lab. 

## Contributors
This program was written by Preston Hodsman based on a request for analysis from Trilogy Education Services, a 2U, Inc.

## License
MIT

# Report

## Overview of the Analysis

In analyzing credit risk using machine learning techniques, due to the small amount of high risk loans in a dataset, it is possible for the results of a machine learning model to not deliver the best results in trying to identify high risk loans in another similar dataset. In this analysis, two machine learning techniques will be compared on a historical data set for lending activity from a peer-to-peer lending services company. The goal is to find which model is better for identifying creditworthiness of borrowers with similar datasets.

The two machine learning methods compared will both use logistic regression on randomly split versions of the original data, with training sets and testing sets. The training set will be used to train the machine learning model, and then the model will be applied to the testing set to see how well it performs in terms of percent of correctly identified high risk loans, and percent of incorrectly identified high risk loans. Since the amount of high risk loans is a small portion of the dataset, a second model will be run using an imbalanced learning approach that oversamples the amount of high risk loans, and the results will be compared.

In the original training split data set, there were 75036 good loans, and 2500 high risk loans. The resampled training split dataset oversamples the high risk loans to get a better dataset for this particular machine learning algorithm of Logistic Regression to work on, which instead has 56271 good loans and 56271 high risk loans.

## Results

The two models are compared on three main metrics. Accuracy, precision, and recall. Accuracy is the percent of correct predictions, which includes the target(high risk loans) and the non-targets(low risk loans). Precision is the percent of predictions of the target which are correct, so it is a way to measure the percent of false positives of the model. Recall is the percent of the targets that are accurately identified, so it is a way to measure how many of the targets are missed. There is often a tradeoff between getting a higher amount of targets correctly identified and overidentifying and creating false positives for this kind of data, so the tradeoff must be measured for the particular application.

- Machine Learning Model 1: Logistical Regression with Train-Test Split
  - Accuracy: 95.2%
  - Precision: 85%
  - Recall: 91%

- Machine Learning Model 2: Logistical Regression with Resampled Train-Test Split
  - Accuracy: 99.4%
  - Precision: 84%
  - Recall: 99%

## Summary

In this case, the Logistical Regression model using Resampled Training data seems significantly superior, with a very small rate of increased false positives. The model using Resampled data correctly identified 99 percent of high risk loans from the test data, compared to the first model which only identified 91 percent of high risk loans, with a tradeoff of only one percent more false positives. 

If one were to compare the costs to the platform of it having a reputation of not warning lenders 9 percent of the time that they are entering into a high risk loan arrangement vs a 1 percent chance of this, and compare this to the tradeoff of having 16 percent of borrowers who are not actually high risk having to go through extra steps or accept higher interest rates to get a loan vs 15 percent, it seems obvious that the tradeoff is significantly better for the platform to adopt the machine learning approach using resampled training data.

What could be better is if more models were tested and a third model was identified that reduced the amount of false positives to a significantly lower amount while retaining the high rate of correct identification of high risk loans.
