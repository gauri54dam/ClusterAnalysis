# ClusterAnalysis
This repo uses K-means algorithm to separate records into different clusters. 
The number of clusters is provided as input parameter to the model. 

About Dataset :
https://www.kaggle.com/datasets/uciml/iris

The input data is taken from Kaggle. This Iris Species dataset classifies iris plants into three species 
1) Setosa - 0
2) Versicolor - 1
3) Virginica - 2

Input dataset has 4 features based on which clustering is done namely-
1) sepal.length	
2) sepal.width	
3) petal.length	
4) petal.width

Step 1 : - Internal Validation

As a part of Unsupervised learning, the last species column is not considered.
The rest of the input dataset is fed to KMeans algorithm with which the data is been divided into clusters.

The Internal validation techniques are employed on the clusters to verify the result.
The clustering evaluation is done to maximize the following coefficients:
1) Calisnki-Harabasz coefficient
2) Dunn index
3) silhouette coefficient

Thus based on analysis for the cluster size 3 gives the maximum values for coefficients.

Step 2 : - External Validation

As a part of Supervised learning, the last species column is considered.
The species values are converted into numbers 0,1,2.
The output values from KMeans algorithm are compared with the actual cluster values (0,1,2) using following techniques :

1) Precision score
2) recall score
3) Jaccard coefficient 
4) Rand coefficient 
5) Folkes and Mallows coefficient 
