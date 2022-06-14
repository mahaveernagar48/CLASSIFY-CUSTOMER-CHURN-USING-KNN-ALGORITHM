# Problem Statement

Imagine a telecommunications provider has segmented its customer base by service usage patterns, categorizing the customers into four groups. If demographic data can be used to predict group membership, the company can customize offers for individual prospective customers. It is a classification problem. That is, given the dataset,  with predefined labels, we need to build a model to be used to predict class of a new or unknown case.

## Objective

Our objective is to build a classifier, to predict the class of unknown cases. We will use a specific type of classification called K nearest neighbour (**KNN**).

**K-Nearest Neighbors** is a supervised learning algorithm. KNN is a method of classifying cases based on thier similarity to other cases. Cases that are near to each other are assigned to a particular class based on thier similarity and disimilarity. Similarity and dissimilarity can be identified by ecludian distance between two class labels.

### K-Nearest Neighbors algorithm graph.

<img src="http://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1531424125/Knn_k1_z96jba.png">
<img src="http://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1531424125/KNN_final1_ibdm8a.png">

In this case, we have data points of Class A and B. We want to predict what class ? (test data point) belong to. If we consider a k value of 3 (3 nearest data points), we will obtain a prediction of Class B. Yet if we consider a k value of 6, we might obtain a prediction of Class A.

KNN has three basic steps.
1. Calculate the distance.
2. Find the k nearest neighbours.
3. Vote for classes
