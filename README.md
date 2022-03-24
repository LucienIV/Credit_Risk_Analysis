# Credit_Risk_Analysis

## Overview

### Overview of the Analysis
The purpose of this analysis is to utilize several different machine learning models to assess a given dataset of credit information from a lending services company, determining which model was the best for predicting credit risk.

## Results

### Naive Random Oversampling
- This model had a balanced accuracy score of ~0.648
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159961461-a4d58263-8104-4fa8-92fa-521d11225ca3.png)

The model had a high precision score for low risk but it had an incredibly low precision score for high risk. Both recall scores were only slightly above average.

### SMOTE Oversampling
- This model had a balanced accuracy score of ~0.627
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159962691-b5299cc2-a241-48de-b717-80ef9a577a72.png)

This model was very similar to the prior oversampling model, with roughly the same precision and recall scores.

### Cluster Centroids Undersampling
- This model had a balanced accuracy score of ~0.516
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159962930-dddd7429-4bee-43e6-bc69-40c65cba3905.png)

Much like the prior two models, the high risk precision score was very low and the low risk precision score was very high. The high risk recall score was slightly above average too, but the recall score for low risk was much lower than in previous models.

### SMOTEEN Combination Sampling
- This model had a balanced accuracy score of ~0.516
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159963270-67a2e73c-7cc4-49a3-8adb-90a3fb76492e.png)

The outcome of this model was exactly identical to the cluster centroids model. 

### Balanced Random Forest Classifier
- This model had a balanced accuracy score of ~0.783
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159963565-d0d621f3-0958-48c2-9b9a-e90a40111883.png)

As with all prior models this model had a high precision score for low risk and a low precision score for high risk. It had markedly better recall scores for both though.

### Easy Ensemble AdaBoost Classifier
- This model had a balanced accuracy score of ~0.931
- The precision and recall scores were as follows:

![image](https://user-images.githubusercontent.com/92831138/159964380-5b27d7c1-0354-4db4-bc7b-95776edf11fb.png)

This model had the best scores of all tested models. As with all prior models the precision score for low risk was high. The high risk precision score for this model was low, but was not as low as the other models. Additionally, the recall scores for both were incredibly high.

## Summary

### Summary and Recommendation of Model
All examined models had many points of similarity. The precision score for predicting low risk was high and the precision score for predicting high risk was low. For the most part the recall scores were above average. Overall, if a recommendation were to be made on a model to use the Easy Ensemble Adaboost Classifier model would be the recommended model. The precision score for high risk predictions was higher than the other models, the precision score for low risk predictions was as high as the other models, this model had the highest balanced accuracy score, and the recall scores for both high and low risk was very high in the model. The only concern with the model is that the low precision score for high risk will lead to a number of false positives.
