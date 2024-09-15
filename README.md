# Marketing-Project
![](images/marketing-introduction.jpg)

---
<img src="images/matplotlib-logo.png" alt="Matplotlib Logo" width="130"/> <img src="images/numpy-logo.png" alt="Numpy Logo" width="130"/> <img src="images/sklearn-logo.png" alt="Sklearn Logo" width="130"/> <img src="images/pandas-logo.jpg" alt="Pandas Logo" width="130"/> <img src="images/seaborn-logo.png" alt="Seaborn Logo" width="130"/>  <img src="images/tensorflow-logo.jpg" alt="Tensorflow Logo" width="130"/> <img src="images/keras-logo.jpg" alt="Keras Logo" width="130"/>

## Introduction
This project focuses on using data science to address a key challenge in marketing area. The idea is to make possible campaigns more targeted and relevant, leading to better results. If the goal of a marketing campaign is to communicate a message to customers, is essencial to address the message to the desired target.

## Problem Statement
This project addresses the problem by developing a machine learning model that segments customers into different groups for future marketing campaigns.

## Background
- Import libraries and datasets
- Visualize dataset
- Data cleaning and exploration
- Exploratory Data Analysis (EDA)
- Definition of numbers of clusters
- K-Means
- Principal Components Analysis (PCA)
- Dimesionality Reduction Using Autoencoders
- Final Model

## Models Used
- Principal Component Analysis (PCA)
- Autoencoders
- K-Means

## Data Sourcing
The dataset used in this project is a cleaned version of information extracted from the internet. 

## Data Cleaning and Exploration
The data was previously cleaned with a first ETL process, the last changes produced to it were:
1) To drop null values in MINIMUM_PAYMENT and CREDIT_LIMIT.
2) To remove unnecessary column such as CUST_ID.
3) To scale all the dataset.

## Exploratory Data Analysis (EDA)
In this step, the principal objective was to:
- To use KDE Plot  for visualizating the probability density of each variable (example).
  ![](images/credit-limit-kdeplot.jpg)
- To graph and understand other correlations in values.
  ![](images/correlations.png)
  
## Definition of Number of Clusters
Prevously to create testing and training datasets, some data must have been scaled, such as categorical features 'BusinessTravel', 'Department', 'EducationField', 'Gender', 'JobRole' and 'MaritalStatus'.
Test size selected was 25%.

## Definition of Numbers of Clusters
The first proof was with 8 as a right number of clusters for the model.

## Principal Components Analysis (PCA)
After graphing each value  represented with the clusters, we can see that the results are not so good.
 ![](images/clusters-proof1.png)
Next step was to reduce the cluster's quantity to an optim final value.

## Autoencoders for Dimensionality Reduction
In this step, the better way to finally reduce the cluster's quantity was with keras and tensorflow designing a neuronal network that endoded and decoded again each feature educing the number of features

TRY TO REALLY UNDERSTAND WHAT IS DOING THE MODEL IN THIS STEP.. SEE THE NEXT RESPONSE OF CHATGPT

---
An autoencoder reduces the dimensionality of the data, not the number of clusters. Here's a breakdown:

Reducing Data Dimensionality: An autoencoder learns a compressed, lower-dimensional representation of the input data through its hidden layers. The goal is to represent the essential features of the data in fewer dimensions, making it easier for algorithms like K-means to find meaningful patterns.

K-means Clustering: After the dimensionality reduction, K-means is applied to the compressed data to form clusters. The number of clusters is still determined by K-means, based on the number of groups you define, not by the autoencoder.

In short, the autoencoder reduces the number of features (dimensionality), while K-means finds clusters in the reduced data.
---




