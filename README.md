# Credit Risk Analysis

## Overview

To Predict Credit Risk with Supervised Machine Learning.

We will resample the dataset, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Purpose

Methods

- Oversampling: RandomOverSampler Algorithm and SMOTE Algorithm

- Undersampling: ClusterCentroids Algorithm

- Combinatorial of over- and undersampling: SMOTEENN Algorithm

- Classifiers: BalancedRandomForestClassifier and EasyEnsembleClassifier

## Results

- RandomOverSampler

The balanced accuracy test it 65%, the precision for the high_risk has a very low positivity at 1% and the recall is 68%.

![Screen Shot 2021-12-11 at 8 51 56 PM](https://user-images.githubusercontent.com/88747464/145697530-13f24fb9-38a2-4fc2-a499-0b69c5045d18.png)

- SMOTE

The balanced accuracy test it 64%, the precision for the high_risk has a very low positivity at 1% and the recall is 66%.

![Screen Shot 2021-12-11 at 8 58 28 PM](https://user-images.githubusercontent.com/88747464/145697567-de8245d8-5be6-44b1-bfd6-693ed6ea8c1d.png)

- ClusterCentroids

The balanced accuracy test it 52%, the precision is 99% and the recall is 43%.

![Screen Shot 2021-12-11 at 8 59 05 PM](https://user-images.githubusercontent.com/88747464/145697589-42ddc2a6-4429-4963-8bfc-addbc48c0eff.png)

- SMOTEENN

The balanced accuracy test it 64%, the precision is 99% and the recall is 57%.

![Screen Shot 2021-12-11 at 8 59 41 PM](https://user-images.githubusercontent.com/88747464/145697588-926b7456-d380-4ef3-8d22-924eacb7a86d.png)

- BalancedRandomForestClassifier

The balanced accuracy test it 67%, the precision for the high_risk is 73% and the recall for the high_risk is 34%. 

![Screen Shot 2021-12-11 at 9 00 49 PM](https://user-images.githubusercontent.com/88747464/145697628-f69efb31-6c50-45a9-989b-af6e16728dc8.png)

- EasyEnsembleClassifier

The balanced accuracy test it 92%, the precision is 99% and the recall is 94%.

![Screen Shot 2021-12-11 at 9 01 40 PM](https://user-images.githubusercontent.com/88747464/145697617-4767a5c0-d4f6-4ba6-8c68-0776cf5e9807.png)

## Summary

For the first four models, we oversampled and undersampled data to determine which model is best at predicting which loans are the highest risk. 

Additionally, we resampled the data using ensemble classifiers to predict which loans are high or low risk. 

In the resampling models, the accuracy scores are around 65%. They are not very high as the ensemble classifiers. The recall scores are typically low as well. 

Thus, I recommend ensemble classifiers over the resampling models. 

Moreover, the Easy Ensemble had the highest accuracy score, which is 92%. The precision and recall scores are also high in good balances. 
