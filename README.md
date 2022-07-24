# Machine Learning from Scratch

## Project Description

In this project we build many different Machine Learning models from scratch. This means that, rather than using the instances provided by the scikit-learn library, we build the models from the ground up, manufacturing ourselves all tools we need. More specifically, for each model we first present a detailed pseudo code of the algorithm that implements it; then we proceed to code each step separately. Once the model is ready, we evaluate its performance using different hyperparameters values; finally, we compare our model to the reference implementation from scikit-learn: in each case both objects yield the same results.

It's important to keep in mind that obtaining small errors and optimal model performances is not the main goal of this project. Hence, some tasks that usually make up an important part of the Machine Learning pipeline (like data visualization and feature selection) are here either overlooked or completely ignored.  

## Project Motivation

Coding from scratch something that is readily available in a popular and easily accessible library like scikit-learn might seem like a tedious and arid exercise. However, the silver lining of this approach is that, by reviewing and putting into action each step of the algorithm, one achieves a clear, intimate understanding of how the related model really works. Moreover, having the entire source code availabe allows higher levels of model customization.

## About the Data

Since the focus of this project is to enahnce my Machine Learning knowledge building models from scratch (rather than analyzing a specific real-world issue), we will for the most part use the toy datasets contained in the `sklearn.datasets` module. The only exception are the Naive Bayes notebook (where we use a collection of 5,572 SMS which is available [here](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)) and the k-Means Clustering notebook (where we use data from the videogame FIFA 22 that can be found [here](https://www.kaggle.com/datasets/stefanoleone992/fifa-22-complete-player-dataset)).  

## Notebooks Overview

- `naive_bayes.ipynb`: we implement a Multinomial Naive Bayes Classifier from scratch to build a filter that determines whether a text messages is spam or not spam (I actually created this notebook a while ago as a separate project; hence, its structure is slightly different compared to the other ones).
- `grad_boost_reg.ipynb`: we implemenet a Gradient Boosting Regressor from scratch. This is a tree based ensemble method which trains weak learners at different stages focusing each time on correcting the errors made during the previous stage.  
- `grad_boost_clf.ipynb`: we implemenet a Gradient Boosting Classifier from scratch. Same as above but this time we solve a (multiclass) classification problem.
- `knn_reg.ipynb`: we implement a k-Nearest Neighbors Regressor from scratch. This uses a distance based algorithm to find the training samples that are closest to the new observations. Predictions are then made by taking the average among these closest samples.
- `knn_clf.ipynb`: we implement a k-Nearest Neighbors Classifier from scratch. Same as above but this time predictions are made using a majority vote among the nearest neighbors.
- `kmeans_clust.ipynb`: we implement a k-Means Clustering algorithm from scratch. This is an unsupervised machine learning technique that allows to cluster data points based on their distance from the centroids.
