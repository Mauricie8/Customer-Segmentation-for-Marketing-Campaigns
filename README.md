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
- To compare dependent variable with less correlated independent variable.
- To graph and understand other correlations in values.







