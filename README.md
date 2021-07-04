# Credit_Risk_Analysis

### Overview and Purpose of the Analysis:

In this project, we will use machine learning to assess credit loan risk. The Scikit-learn library will allow us to build and evaluate several supervised machine learning models to predict credit risk. Analysing credit risk has an unbalanced classification problem due to good loans outnumbering risky loans so I will use oversampling (such as RandomOverSampler and SMOTE), undersampling (ClusterCentroids) and ensemble algorithms. I will compare the strengths and weaknesses of the different machine learning models and determine whether they are useful in predicting credit risk. The objective of this analysis is to assess how well each model classifies and predicts credit risk and whether the imbalance between high-risk and low-risk data can be overcome in the various models.

##

### Results:

 Model:   |      Results:   |   |
|----------|:-------------:|:-------------|
|Naive Random Oversampling |  ![naive](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/naive_random_oversampling.png) | |
| Smote Oversampling|  ![smote](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smote_oversampling.png)  |   |
| Cluster Centroids Undersampling |  ![cluster](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/cluster_centroids_undersampling.png)  |  |
| Smooteenn Combination Sampling |  ![smoteen](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smoteenn.png)  |      |
| Balanced Random Forest Classifier |   ![forest](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/balanced_forest_del3ensemble.png)   |  |  
| Easy Ensemble Classifier |  ![easy](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/easy_ensemble_del3.png)   |    |
