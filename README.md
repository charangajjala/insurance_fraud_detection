# insurance_fraud_detection
Problem Statement: To build a classification methodology to determine whether a customer is placing a fraudulent insurance claim.

## Architecture:
![image](https://user-images.githubusercontent.com/64437927/194085358-b90ab54a-1758-4548-8fdd-44275d68a496.png)

## Methodology:
Clustering - KMeans algorithm is used to create clusters in the preprocessed data. The optimum number of clusters is selected by plotting the elbow plot, and for the dynamic selection of the number of clusters, we are using "KneeLocator" function. The idea behind clustering is to implement different algorithms
The Kmeans model is trained over preprocessed data, and the model is saved for further use in prediction.
Model Selection – After the clusters have been created, we find the best model for each cluster. We are using two algorithms, “SVM” and "XGBoost". For each cluster, both the algorithms are passed with the best parameters derived from GridSearch. We calculate the AUC scores for both models and select the model with the best score. Similarly, the model is selected for each cluster. All the models for every cluster are saved for use in prediction.



