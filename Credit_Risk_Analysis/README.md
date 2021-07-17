# Credit_Risk_Analysis

## Project Overview
FinTech firms are storming ahead of traditional loan processes. By using the latest 
machine learning techniques, these FinTech firms can continuously analyze large 
amounts of data and predict trends to optimize lending.

In this module, you’ll use Python to build and evaluate several machine learning models
to predict credit risk. Being able to predict credit risk with machine learning 
algorithms can help banks and financial institutions predict anomalies, reduce risk 
cases, monitor portfolios, and provide recommendations on what to do in cases of fraud

## Resources
- **Data Source:** LoanStats_2019Q1.csv
- **Software:** Python and Scikit-learn 

## Objective
- Explain how a machine learning algorithm is used in data analytics.
- Create training and test groups from a given data set.
- Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
- Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
- Compare the advantages and disadvantages of each supervised learning algorithm.
- Determine which supervised learning algorithm is best used for a given data set or scenario.
- Use ensemble and resampling techniques to improve model performance.

## Summary
Machine learning is the use of statistical algorithms to perform tasks such as 
learning from data patterns and making predictions. There are many different models—a 
model is a mathematical representation of something that happens in the real world

## Supervised Learning
Supervised learning deals with labeled data. An example of supervised learning might 
be to predict, based on data from previous patientw, whether a new patient has diabetes.
Supervised learning can be broadly divided into "Regression" and "Classification"

## Regression:
- Population Growth Prediction
- Advetising Popularity prediciton
- Life Expectancy Prediction

## Regression: Used to predict continuous variables
let’s say that we’re interested in predicting a person’s weight based on factors like 
height, dietary preferences, and exercise patterns. To do this we would collect data on
a number of people. The regression model’s algorithms would attempt to learn 
patterns that exist among these factors.

## Regression vs. Classification
There is a major difference between regression and classification models. 
In our regression example, the target variable, or what we’re trying to predict, 
is weight. Weight is a continuous variable—a person’s weight can be any numerical 
value within a certain range. In our classification example, on the other hand, 
the target variable only has two possible values; whether a person votes “Yes” or “No.” 
When the classification model encounters new data, it would attempt to predict 
whether the votes cast by people will be “Yes” or “No.”

## Classification
Classification, on the other hand, is used to predict discrete outcomes. 
For example. Let’s say that we are interested in using a person’s traits, such as age, 
sex, income, and geographic location, to predict how she or he will vote on a particular issue. 
The outcome, in this case, is whether the person will vote “Yes” or “N

## Unsupervised Learning
In unsupervised learning, by contrast, machine learning algorithms work with datasets 
without labeled outcomes. In supervised learning, the labels provide the correct answers. 
In unsupervised learning, such correct answers, or labels, aren’t provided
A common application of unsupervised learning is to group customers by purchasing patterns.

# Credit Risk Challenge

## Background
Credit risk is an inherently unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Your final task is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Objectives
- Implement machine learning models.
- Use resampling to attempt to address class imbalance.
- Evaluate the performance of machine learning models.

## Instructions
You’ll use the imbalanced-learn library to resample the data and build and evaluate logistic regression classifiers using the resampled data. Download the files you’ll need, which include starter code and the datase

## Perform Analysis:
- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the cluster centroids algorithm.
- Use a combination approach with the SMOTEENN algorithm.
- Train a logistic regression classifier (from Scikit-learn) using the resampled data.
- Calculate the balanced accuracy score using balanced_accuracy_score from sklearn.metrics.
- Generate a confusion_matrix.
- Print the classification report (classification_report_imbalanced from imblearn.metrics).

Lastly, you’ll write a brief summary and analysis of the models’ performance. Describe the precision and recall scores, as well as the balanced accuracy score. Additionally, include a final recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning

## Extension
For the extension, you’ll train and compare two different ensemble classifiers to predict loan risk and evaluate each model. Note that you’ll use the following modules, which you have not used before. They are very similar to ones you’ve seen: BalancedRandomForestClassifier and EasyEnsembleClassifier, both from imblearn.ensemble. These modules combine resampling and model training into a single step

## Use 100 estimators for both classifiers, and complete the following steps for each model:
- Train the model and generate predictions.
- Calculate the balanced accuracy score.
- Generate a confusion matrix.
- Print the classification report (classification_report_imbalanced from imblearn.metrics).
- For the BalancedRandomForestClassifier, print the feature importance, sorted in descending order (from most to least important  feature), along with the feature score.

Lastly, you’ll write a brief summary and analysis of the models’ performance. Describe the precision and recall scores, as well as the balanced accuracy score. Additionally, include a final recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
