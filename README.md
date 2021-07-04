# Credit_Risk_Analysis

### Overview and Purpose of the Analysis:

In this project, we will use machine learning to assess credit loan risk. The Scikit-learn library will allow us to build and evaluate several supervised machine learning models to predict credit risk. Analysing credit risk has an unbalanced classification problem due to good loans outnumbering risky loans so I will use oversampling (such as RandomOverSampler and SMOTE), undersampling (ClusterCentroids) and ensemble algorithms. I will compare the strengths and weaknesses of the different machine learning models and determine whether they are useful in predicting credit risk. The objective of this analysis is to assess how well each model classifies and predicts credit risk and whether the imbalance between high-risk and low-risk data can be overcome in the various models.

##

### Results:

The table below, show the results of each machine learning models and the bulleted list discusses the results of each model.

* Naive Random Oversampling:
  * The Naive Random Oversampling model had a recall value of 0.45 and precision value of 0.01 in predicting high risk loans and an accuracy score of 0.58. 
  * This model performed the worst overall as it achieved the second lowest accuracy score and lowest recall and precision values in predicting high risk loans.

* Smote Oversampling:
  * The Smote Oversampling model performed slightly better than the Naive Random Oversampling model in terms of accuracy. It's balanced accuracy score was 0.63 which is just slightly higher than the Naive Random model (0.58) due to having a higher number of true positives in the confusion matrix.
  * Overall, the Smote model performed very similarly to the Naive Random model when it comes to predicting high risk loans as it achieved similar low scoring recall (0.54) and precision values (0.01).

* Cluster Centroids Undersampling:

 Model:   |      Results:   |   
|----------|:--------:|
|Naive Random Oversampling |  ![naive](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/naive_random_oversampling.png) 
| Smote Oversampling|  ![smote](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smote_oversampling.png)  
| Cluster Centroids Undersampling |  ![cluster](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/cluster_centroids_undersampling.png)  
| Smooteenn Combination (Over and Under) Sampling |  ![smoteen](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smoteenn.png)      
| Balanced Random Forest Classifier |   ![forest](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/balanced_forest_del3ensemble.png)     
| Easy Ensemble Classifier |  ![easy](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/easy_ensemble_del3.png)      
