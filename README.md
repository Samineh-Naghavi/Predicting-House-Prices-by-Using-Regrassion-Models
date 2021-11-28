# Predicting House Prices by Using Regression Models
## Supervised Learning
Supervised learning is the most common subbranch of machine learning (ML) today. Typically, new machine learning practitioners will begin their journey with supervised learning algorithms. Supervised machine learning algorithms are designed to learn by example. The name “supervised” learning originates from the idea that training this type of algorithm is like having a teacher supervise the whole process. When training a supervised learning algorithm, the training data will consist of inputs paired with the correct outputs. During training, the algorithm will search for patterns in the data that correlate with the desired outputs. After training, a supervised learning algorithm will take in new unseen inputs and will determine which label the new inputs will be classified as based on prior training data. 

The objective of a supervised learning model is to predict the correct label for newly presented input data. At its most basic form, a supervised learning algorithm can be written simply as:

<br /> **Y = F(X)** 
 
Where Y is the predicted output that is determined by a mapping function that assigns a class to an input value x. The function used to connect input features to a predicted output is created by the machine learning model during training.

Supervised learning uses a training set to teach models to yield the desired output. This training dataset includes inputs and correct outputs, which allow the model to learn over time. The algorithm measures its accuracy through the loss function, adjusting until the error has been sufficiently minimized. Supervised learning can be separated into two types of data mining problems; classification and regression, where the regression is explaied in this section.

## Regression
Regression is used to understand the relationship between dependent and independent variables. It is commonly used to make projections, such as for sales revenue for a given business. Linear regression, logistical regression, and polynomial regression are popular regression algorithms.

### Simple Linear Regression
This is one of the most common and interesting type of Regression technique to predict a target variable Y based on the input variable X. A linear relationship should exist between target variable and predictor, reflecting the name of Linear Regression.

For example, consider predicting the House Price based on the number of it's bedrooms. It can be easily identified that there seems to be a correlation between bedrooms number and house price (more bedrooms, more the house price). The hypothesis of linear regression is

<br /> **Y = a + bX**
 
Y represents house price, X is bedroom number and a and b are the coefficients of the equation. To predict Y (price) given X (bedroom number), the values of a and b (the model’s coefficients) needs to be known.

### Multiple Linear Regression
Multiple linear regression (MLR), also known as multiple regression, is a statistical technique that uses several explanatory variables to predict the outcome of a response variable. The goal of multiple linear regression is to model the linear relationship between the explanatory (independent) variables and response (dependent) variables. In essence, multiple regression is the extension of ordinary least-squares regression because it involves more than one explanatory variable. 

<br /> **Y = a + bX1 + bX2 + bX3 + ...+ bXn**

### Polynomial Regression
In polynomial regression, the original features are transformed into polynomial features of a given degree and then apply Linear Regression on it. Consider the above linear model Y = a+bX is transformed into 

<br /> **Y=a + bX +cX^2**

### Random Forest Regression
Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time. A Random Forest operates by constructing several decision trees during training time and outputting the mean of the classes as the prediction of all the trees. In fact Random Forest is an ensemble learning method that combines predictions from multiple machine learning algorithms to make a more accurate prediction than a single model.

A Random Forest Regression model is powerful and accurate. It usually performs great on many problems, including features with non-linear relationships. Disadvantages, however, include, no interpretability, overfitting may easily occur, and the number of trees to include in the model needs to be chosen.

To get a better understanding of the Random Forest algorithm, following steps are required to be completed:

<br /> 1.	Pick at random k data points from the training set.
<br /> 2.	Build a decision tree associated to these k data points.
<br /> 3.	Choose the number N of trees you want to build and repeat steps 1 and 2.
<br /> 4.	For a new data point, make each one of your N-tree trees predict the value of y for the data point in question and assign the new data point to the average across all of the predicted y values.

### Support Vector Regression (SVR)
In SVR, a hyperplane with maximum margin is identified such that the maximum number of data points are within that margin. SVRs are almost similar to the SVM classification algorithm. We will discuss the SVM algorithm in detail in classification (See main page). Instead of minimizing the error rate as in simple linear regression, the error is fitted within a certain threshold. The objective in SVR is to consider the points that are within the margin, where the best fit line is the hyperplane that has the maximum number of points.

## Pros and Cons of various Machine Learning Regression algorithms

![](images1.jpg)

***In order to choose the best model, the performance of each model on the selected dataset is carefully considered.***
 
## K-fold Cross-Validation
The k-fold cross-validation procedure is a standard method for estimating the performance of a ML algorithm or configuration on a dataset. Cross-validation is used to detect overfitting and failing to generalize a pattern. In the regression model, it used to find the best squared by using the optimal hyper parameters. The performance measure reported by k-fold cross-validation is then the average of the values computed in the loop. This approach can be computationally expensive, but does not waste too much data (e.g., when fixing an arbitrary validation set), which is a major advantage in problems such as inverse inference where the number of samples is very small (See below).

![](grid_search_cross_validation.jpg)

## Dataset Explanation 
The real estate markets present an interesting opportunity for data analysts to analyze and predict where property prices are moving towards. Prediction of property prices is becoming increasingly important and beneficial. Property prices are a good indicator of both the overall market condition and the economic health of a country. Considering the data provided by Kaggle .com, a large set of property sales records are stored in an unknown format and with unknown data quality issues.

This repository contains Python implementation of the supervised learning algorithms devised in the Supervised Learning Algorithms for Predicting House Prices by using Regression Models to predict the final price of each home.

![](images.jpg)

#### Objectives
<br /> •	Create feature engineering 
<br /> •	Advanced regression techniques like random forest, SVR and Linear Regression models
 
