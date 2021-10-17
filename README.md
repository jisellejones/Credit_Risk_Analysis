# Credit_Risk_Analysis

* Repo photo by [Avery Evans](https://unsplash.com/@averye457?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on Unsplash

## Overview
The purpose of this analysis was to predict credit risk by employing different techniques to train and evaluate models with unbalanced classes on a credit card credit dataset. We ran logical regression:

### Data Source
  - LendingClub
    - LoanStats_2019Q1.csv

### Software/Libraries
  - python 3.7
  - scikit-learn vs 0.24.1
  - imbalacned-learn vs 0.8.1
  - Jupyter Notebook vs 6.3.0

## Results

- The model with the highest accuracy score was the Easy Ensemble Classifier at 0.93.
- Precision scores were low for all models with easy ensemble classifier predicting high risk credit applications at 0.07.
- The easy ensemble classifier boosted predicted high risk credit applications with 0.94 specificty and low risk credit applications 0.91 specificity.
- When considering the f1 score, all models performed poorly at predicting high risk credit applications, the highest f1 score being 0.02.

*Accuracy of all Models*
|   Model | Accuracy|
|---------|---------|
|Naive Random Oversampling| 0.65 |
|SMOTE Oversampling| 0.64  |
|Undersampling - Cluster Centroids| 0.53 |
|Combination Sampling | 0.64 |
|Balanced Random Forest Classifier| 0.79 |
|Easy Ensemble Classifier| 0.93 |

### Resampled Logistic Regression Models

*Naive Random Oversampling Classification Report*
![Naive_random_oversampling](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/random_over_sampling.png)

*SMOTE Oversampling Classification Report*
![SMOTE_oversampling](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/smote_over_sampling.png)

*Undersampling using the Cluster Centroids Algorithm Classification Report*
![undersampling_cluster_centroids](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/undersampling.png)

*Combination Sampling Classification Report*
![combination_sampling](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/combination_sampling.png)

### Ensemble Models
*Balanced Random Forest Classifier Classification Report*
![balanced_random_forest_classifier](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/balanced_random_forest_classifier.png)

*Easy Ensemble Classifier Classification Report*
![easy_ensemble_classifier](https://github.com/jisellejones/Credit_Risk_Analysis/blob/main/Images/easy_ensemble_classifier.png)

## Summary

Due to the high accuracy and specificity scores of the Easy Ensemble Classifier, we recommend this model to predict high risk credit applications using specficity scores to predict both high risk credit applications and low risk credit applications.
