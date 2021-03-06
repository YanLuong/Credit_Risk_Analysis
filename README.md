# Credit Risk Analysis

### Overview and Purpose of the Analysis:

In this project, we will use machine learning to assess credit loan risk. The Scikit-learn library will allow us to build and evaluate several supervised machine learning models to predict credit risk. Analysing credit risk has an unbalanced classification problem due to low risk credit outnumbering risky credit so I will use oversampling (such as RandomOverSampler and SMOTE), undersampling (ClusterCentroids) and ensemble algorithms. I will compare the strengths and weaknesses of the different machine learning models and determine whether they are useful in predicting credit risk. The objective of this analysis is to assess how well each model classifies and predicts credit risk and whether the imbalance class distribution between high-risk and low-risk data can be overcome in the various models.

##

### Results:

Refer to the table below for the results of each machine learning models and the bulleted list discusses the results of each model.

* Naive Random Oversampling:
  * The Naive Random Oversampling model had a recall value of 0.45 and precision value of 0.01 in predicting high risk loans and an accuracy score of 0.58. 
  * This model performed second worst overall as it achieved the second lowest accuracy score and lowest recall and precision values in predicting high risk credit.
  * This model has high precision of 1 in low risk prediction and low recall of 0.71 which means a proportion of credit risk that was predicted to be high risk was actually low risk and not captured correctly. This can be seen in the confusion matrix where there are 4988 false negatives.

* Smote Oversampling:
  * The Smote Oversampling model performed slightly better than the Naive Random Oversampling model in terms of accuracy. It's balanced accuracy score was 0.63 which is just slightly higher than the Naive Random model (0.58) due to having a higher number of true positives in the confusion matrix.
  * Overall, the Smote model performed very similarly to the Naive Random model when it comes to predicting high risk credit as it achieved similar low scoring recall (0.54) and precision values (0.01). Both models have very similar numbers in the confusion matrix.

* Cluster Centroids Undersampling:
  * The Cluster Centroid model performed the worst out of all the models with the lowest scores in precision, recall, F1 and accuracy. It's balanced accuracy is very low at 0.53 and recall is equally low at 0.53 for predicting low and high risk credit. 
  * This model also has the highest number of false negatives of 7955 which is reflected in the low recall.

* Smoteenn Combination Sampling:
  * The Smoteenn Combination Sampling model has a 0.64 balanced accuracy score. It has one of the higher accuracy scores in the sampling models. 
  * The Smoteenn model also has a decent recall score of 0.72 in predicting actual high risk credit correctly while in predicting low risk credit it had a lower recall of 0.57. This can be observed in the confusion matrix where there was 7287 incorrectly predicted high risk loans (false negatives).
  * Like the other sampling methods, Smoteenn model has a high precision score of 1 in predicting low risk credit.
  
* Balanced Random Forest Classifier:
   * The Balanced Random Forest Classifier has much higher balanced accuracy score of 0.78 in comparison to the sampling methods.
   * The recall scores for predicting high risk (0.7) and low risk (0.87) loans are quite balanced and higher on average compared to the sampling methods.
   * While all the previous sampling models had a precision score of 0.01 in high risk, the Balanced Random Forest model performed slightly better in this aspect with a precision score of 0.03. 
   * This classifier has a high F1 score in low risk credit which is significantly better than the sampling methods.

* Easy Ensemble Classifier:
  * The Easy Ensemble Classifier model achieved the highest score in accuracy, precision, recall and F1 out of all the models. It has an accuracy score of 0.93 which is much higher than the Balanced Random Forest model.
  * Recall scores are quite high for low (0.94) and high risk (0.92) credit.
  * In classifying low risk credit, the F1 score is very high at 0.97 while classifying high risk credit the F1 score is low at 0.16. But at 0.16 it is still the highest compared to the previously discussed models.


  

 Model:   |      Results:   |   
|----------|:--------:|
|Naive Random Oversampling |  ![naive](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/naive_random_oversampling.png) 
| Smote Oversampling|  ![smote](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smote_oversampling.png)  
| Cluster Centroids Undersampling |  ![cluster](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/cluster_centroids_undersampling.png)  
| Smoteenn Combination (Over and Under) Sampling |  ![smoteen](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/smoteenn.png)      
| Balanced Random Forest Classifier |   ![forest](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/balanced_forest_del3ensemble.png)     
| Easy Ensemble Classifier |  ![easy](https://github.com/YanLuong/Credit_Risk_Analysis/blob/main/screenshots/easy_ensemble_del3.png)      

##

### Summary: 

* The models that performed the worst are Cluster Centroid and Naive Random. They both have very low accuracy scores, poor recall scores and very high number of false negatives. 
* The ensemble classifier models performed better on the whole when compared to the sampling methods with the Easy Ensemble Classifier achieving highest scores in accuracy, precision, recall and F1 overall. 
* The Easy Ensemble classifier was the model that had lowest number of false negatives and false positives which is indicated by the high balanced accuracy score of 0.93.

### Recommendation:

Based on the results discussed, I would recommend Easy Ensemble Classifier for predicting credit risk. The model is not perfect and may have some overfitting issues but basing it purely on accuracy score then Easy Ensemble model is the more accurate model. It also had the lowest number of false negatives and false positives out of all the models.

