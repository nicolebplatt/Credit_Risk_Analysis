# Credit Risk Analysis

## Overview of Analysis
The purpose of this analysis is to apply different sampling algorithms and machine learning models to a credit card dataset in order to predict credit card risk for a particular lending company.

## Results
The following section reveals the results of our analysis including a synopsis of the balanced accuracy, precision, and recall scores for the four sampling algorithms and two supervised machine learning models.

### Random Oversampling
Using random oversampling, our model produced the following:
- Balanced accuracy score: 0.6447
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: almost identical sensitivity for both high- (0.66) and low-risk (0.62) applicants

### SMOTE
Using SMOTE, our model produced the following:
- Balanced accuracy score: 0.6515
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: almost identical sensitivity for both high- (0.61) and low-risk (0.69) applicants

### Cluster Centroids
Using cluster centroids, our model produced the following:
- Balanced accuracy score: 0.5447
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: better sensitivity for high-risk applicants than low-risk (0.69 vs 0.40)

### SMOTEEN
Using SMOTEEN, our model produced the following:
- Balanced accuracy score: 0.6401
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: better sensitivity for high-risk applicants than low-risk (0.70 vs 0.58)

### Balanced Random Forest Classifier
Using balanced random forest classifier, our model produced the following:
- Balanced accuracy score: 0.8735
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: better sensitivity for low-risk applicants than high-risk (0.87 vs 0.70)

### Easy Ensemble Classifier
Using easy ensemble classifier, our model produced the following:
- Balanced accuracy score: 0.9422
- Precision scores: low precision for high-risk applicants but high precision for low-risk applicants
- Recall scores: almost identical sensitivity for both high- (0.92) and low-risk (0.94) applicants

## Summary
Based on the above results, I would recommend the Easy Ensemble Classifier (EEC) model to use for determining credit risk. While all six models produced very poor precision results for high-risk applicants, the accuracy of the EEC model is a 0.94, the highest of all six models. Additionally, the EEC produced high recall (or sensitivity) scores for both high- and low-risk applicants. Although the EEC (along with the other five models) is not very reliable at high-risk classification (precision), the EEC does provide confidence that it will find all of the high-risk samples.