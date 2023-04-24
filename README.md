# README

## Introduction
This notebook compares the performance and accuracy of the top 10 different types of machine learning algorithms for Classification on the same dataset without any exploratory data analysis done. The goal is to present the 10 most popular classification algorithms.

The following classification algorithms are compared:
- Logistic Regression
- Random Forest
- Support Vector Machines (SVM)
- Gradient Boosting
- Decision Tree
- Neural Network Regression
- KNN Model
- Naive Bayes
- Voting Classification
- Boosting Decision Tree
- XGBRegressor

Cross-validation is used to obtain an overview of the models' scores.

## Dependencies
The following packages are used in this notebook:
- pandas
- matplotlib
- sklearn
- xgboost

## Data
The dataset used in this notebook is the Titanic dataset, available on Kaggle. The training dataset is loaded using the `read_csv` function from the pandas package.

## Feature Selection
The following features are selected for the models:
- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare

## Data Cleaning
The data is cleaned using pipelines, where categorical features are encoded using the `OrdinalEncoder` from the sklearn package and numerical features are imputed using the `KNNImputer` and then standardized using the `StandardScaler`.

## Results
The following models are trained and their performance is compared using cross-validation:
- Logistic Regression
- Naive Bayes
- KNN
- Random Forest

The mean and standard deviation of the scores obtained by the models are as follows:
- Logistic Regression: mean=0.7898, std=0.0307
- Naive Bayes: mean=0.7850, std=0.0342
- KNN: mean=0.8025, std=0.0261
- Random Forest: mean=0.8226, std=0.0375

## Conclusion
Based on the cross-validation scores obtained in this notebook, the Random Forest model performs the best on the Titanic dataset. However, it is important to note that this dataset is relatively small and simple, and the results may differ on larger and more complex datasets.
