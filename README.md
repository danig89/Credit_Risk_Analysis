# Credit_Risk_Analysis

## Purpose
The purpose of this project was to use machine learning to help Fast Lending predict credit risk and accurately identify good candidates for loans. The objectives were:
- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
- Evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
- Data Source: [Loan Stats 2019, First Quarter](Resources/LoanStats_2019Q1.csv)
- Software: Anaconda version 4.9.2; Jupyter Notebook version 6.0.3

## Results

### Balanced Random Forest Classifier
- Balanced accuracy score: 79%
- Precision score: 0.99
- Recall score: 0.87

This model demonstrated high precision and moderately high recall. The model can predict credit risk farely well, but it is highly accurate when it does. 

<b>Balanced Random Forest Classifier Model</b>
<br>
<img src="Resources/balanced_random.png" width="700" height="400"/>

### Easy Ensemble AdaBoost Classifier
- Balanced accuracy score: 93%
- Precision score: 0.99
- Recall score: 0.94

This model demonstrated high precision and high recall. The model is nearly perfect at predicting credit risk.

<b>Easy Ensemble AdaBoost Classifier Model</b>
<br>
<img src="Resources/easy_ensemble.png" width="700" height="400"/>

### Naive Random Oversampling
- Balanced accuracy score: 66%
- Precision score: 0.99
- Recall score: 0.58

This model demonstrated high precision and low recall. The model cannot predict credit risk well, but it is highly accurate when it does.

<b>Naive Random Oversampling Model</b>
<br>
<img src="Resources/naive_oversampling.png" width="700" height="400"/>

### Synthetic Minority Oversampling Technique (SMOTE)
- Balanced accuracy score: 65%
- Precision score: 0.99
- Recall score: 0.68

This model demonstrated high precision and low recall. The model cannot predict credit risk well, but it is highly accurate when it does.

<b>SMOTE Model</b>
<br>
<img src="Resources/smote.png" width="700" height="400"/>

### Cluster Centroids Undersampling
- Balanced accuracy score: 54%
- Precision score: 0.99
- Recall score: 0.40

This model demonstrated high precision and low recall. The model cannot predict credit risk well, but it is highly accurate when it does.

<b>Cluster Centroids Model</b>
<br>
<img src="Resources/cluster_undersampling.png" width="700" height="400"/>

### Combination Oversampling and Undersampling
- Balanced accuracy score: 54%
- Precision score: 0.99
- Recall score: 0.57

This model demonstrated high precision and low recall. The model cannot predict credit risk well, but it is highly accurate when it does.

<b>Combination Model</b>
<br>
<img src="Resources/combo_sampling.png" width="700" height="400"/>

## Summary
It is recommened that to accurately predict credit risk, the Easy Ensemble AdaBoost Classifier model is used. With an accuracy score of 93%, this model will perform well in predicting false positives. The models that should not be used include: Naive Random Oversampling, SMOTE, Cluster Centroids Undersampling, and Combination Oversampling and Undersampling. These models may result in more false negatives, which means more people who are high risk borrowers being classified as low risk.
