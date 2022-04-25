# Credit_Risk_Analysis
## Overview
### Purpose
We are finding credit risk by using different techniques to train and evaluate models with unbalanced classes as we've been asked to use the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We are evaluating the performance of these models to write a recommendation on whether they should be used to predict credit risk.
## Results
### Naive Random Oversampling
![Naive Random Oversampling](https://user-images.githubusercontent.com/92561938/165187108-13dd3869-cf99-4bf3-8435-c8c7e802f835.png)

Balanced accuracy score: 0.6504008094916134

High Risk Performance
- Precision: 0.01
- Recall: 0.68

Low Risk Performance
- Precision: 1.00
- Recall: 0.62

### SMOTE Oversampling
![SMOTE Oversampling](https://user-images.githubusercontent.com/92561938/165187158-eaaa96b6-0e04-46b6-a405-eda62fff5250.png)

Balanced accuracy score: 0.6583599806425919

High Risk Performance
- Precision: 0.01
- Recall: 0.63

Low Risk Performance
- Precision: 1.00
- Recall: 0.68

### Undersampling
![Undersampling](https://user-images.githubusercontent.com/92561938/165187189-cb88938a-940e-4df2-8a9d-16e3c3a0274d.png)

Balanced accuracy score: 0.5442661782548694

High Risk Performance
- Precision: 0.01
- Recall: 0.69

Low Risk Performance
- Precision: 1.00
- Recall: 0.40

### Combination (Over and Under) Sampling
![Combination Sampling](https://user-images.githubusercontent.com/92561938/165187222-0813ebe0-4af7-4a4d-8f27-55ac6ddf491f.png)

Balanced accuracy score: 0.6449163069955265

High Risk Performance
- Precision: 0.01
- Recall: 0.72

Low Risk Performance
- Precision: 1.00
- Recall: 0.57

### Balanced Random Forest Classifier
![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/92561938/165187247-9d384dd0-a9ee-4c31-ae52-d7d37f0fb8b3.png)

Balanced accuracy score: 0.7885466545953005

High Risk Performance
- Precision: 0.03
- Recall: 0.70

Low Risk Performance
- Precision: 1.00
- Recall: 0.87

### Easy Ensemble AdaBoost Classifier
![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/92561938/165187274-aad69064-0d09-45e7-a51b-a66207622a1e.png)

Balanced accuracy score: 0.9316600714093861

High Risk Performance
- Precision: 0.09
- Recall: 0.92

Low Risk Performance
- Precision: 1.00
- Recall: 0.94

## Summary
Using F1 = 2(Precision * Sensitivity)/(Precision + Sensitivity), these are the following calculations:

Naive Random Oversampling
- 0.01972222222
- 0.75

SMOTE Oversampling
- 0.0196875
- 0.81656804733

Undersampling
- 0.01971428571
- 0.57142857142

Combination (Over and Under) Sampling
- 0.01972602739
- 0.72611464968

Balanced Random Forest Classifier
- 0.05753424657
- 0.93048128342

Easy Ensemble AdaBoost Classifier
- 0.16396039604
- 0.96907216494

With these calculations, it shows the best model is the Easy Ensemble AdaBoost Classifier and the worst model is Undersampling. I believe the Easy Ensemble AdaBoost Classifier is recommended for predicting credit risk for this analysis.
