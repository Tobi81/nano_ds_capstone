# Udacity Data Scientist Nanodegree - Capstone Project

### Motivation:
This project applies Machine Learning algorithms to get information about potential customers out of demographic data. It is part of the Udacity Data Scientist Nanodegree and shows the main steps to solve the underlying business needs: data understanding, data preparation, modelling and evaluation. The data and outline of this project was provided by Arvato Financial Solutions, a Bertelsmann subsidiary.

The whole project was divided into four parts:

In Part 0 the provided data is read in and all necessary Data Preparation steps are done.

In Part 1 the demographic data of the company’s existing customers and the general population of Germany are compared with each other. Therefore unsupervised learning techniques are used to identify the parts of the population that best describe the core customer base of a mail-order company.

In Part 2 another dataset with demographic information for targets of a marketing campaign of the company is provided. To predict which individuals are most likely to convert into becoming customers for the company supervised learning techniques are applied.

In Part 3 the supervised learning model built in Part 2 is used to predict the response of a testing data set. This prediction is used to compete in a Kaggle competition.

### Results:
It was necessary to apply the majority of CRISP-DM (CRoss-Industry Standard Process for Data Mining) to both parts of the project. Business Understanding was slipped in as part of the problem description, but Data Understanding, Data Preparation, Modelling and Evaluation had to be developed from scratch. The general rule that Data Preparation is the most time consuming part in the process could be verified once again.

Part 1 showed how unsupervised learning techniques — namely PCA and Clustering with KMeans — were applied to distinguish groups of individuals that best describe the core customer base of the mail-order company. A supervised learning model, in form of LogisticRegression, then helped to identify the main characteristics of these individuals.

Part 2 showed the straightforward way of building a supervised learning model. The base performance of various classifiers was determined. With the help of GridSearchCV the most promising one — GradientBoostingClassifier — was fitted respectively tuned to the training dataset (considering stratified cross-validation) and its performance was evaluated via ROC AUC. A short analysis of the most important features completed the model creation before using it for predicting on the testing dataset which individuals of a marketing campaign are most likely to convert into becoming customers.

### Want to read more?
You can find the corresponding blog post here:
https://medium.com/@tobias.gorgs/how-to-use-machine-learning-for-customer-acquisition-bcd52f42042d

You can find the results of the Kaggle competition here:
https://www.kaggle.com/c/udacity-arvato-identify-customers/leaderboard

### What's included:
Within the repository you'll find the following files:

* Arvato Project.ipynb # Jupyter notebook containing the whole project

* features.csv # Listing of feature names, types and missing values

* README.md

### Libraries used:
The Jupyter notebook is written in Python. Main library used are:

* numpy: scientific computing

* pandas: data structures and data analysis tools

* scikit-learn: Machine Learning