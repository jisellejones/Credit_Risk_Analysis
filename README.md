# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to predict credit risk by employing different techniques to train and evaluate models with unbalanced classes on a credit card credit dataset. We ran logical regression:
- 

## Data Source
  - LendingClub
    - LoanStats_2019Q1.csv

## Software/Libraries
  - python 3.7
  - scikit-learn vs 0.24.1
  - imbalacned-learn vs 0.8.1
  - Jupyter Notebook vs 6.3.0

## Results


### Accuracy of all Models
|   Model | Accuracy|
|---------|---------|
|Naive Random Oversampling|   |
|SMOTE Oversampling|   |
|Undersampling - Cluster Centroids| |
|Combination Sampling | |


### Resampled Logistic Regression Models

- All regression models predicted high risk credit applications at 0.01 precision.
- The naive rand model predicted high risk credit applications the highest at 0.68 specificity with the undersampling using cluster centroids algorithm model performing the lowest at 0.45 specicity.
- When considering the f1 score, all models performed poorly at predicting high risk credit applications, the highest f1 score being 0.02.



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
