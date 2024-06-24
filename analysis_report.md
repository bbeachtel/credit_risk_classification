### Analysis Report

### Overview
I conducted an analysis using machine learning models to predict outcomes based on financial data. The purpose of this analysis was to develop predictive models that could assist in assessing risk associated with loans.

The financial data included various attributes such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. 

The target variable we aimed to predict was the loan risk category, where 1 represents a high-risk loan and 0 indicates a healthy loan.

### Basic Information about the Variables
Here is a summary of the target variable distribution (value_counts):

0 (healthy loan): 56271 instances
1 (high-risk loan): 1881 instances
Stages of the Machine Learning Process
The machine learning process involved several stages:

## Data Preprocessing: 
This included reading the csv data into a Pandas DataFrame, and defining what columns to use for the Split_Train_Test. In this dataset, it made sense to define 'loan_status' as our labels and all other columns as the features.

## Model Selection: 
It made sense to start with a simple logistical regression model with this dataset in order to get a baseline performance level of the model.

## Model Evaluation: 
I used a confusion matrix and classification report to understand key metrics about the model's performance.

After evaluating the logistical regression model, I decided to instantiate a LazyClassifier model to quickly see how other models performed with the dataset.

## Methods Used
I employed the following methods as part of the analysis:
    - train_test_split
    - LogisticRegression
    - confusion_matrix
    - classification_report
    - LazyClassifier

## Recommendation
From my analysis, I found most models tested in the LazyClassifier method to perform as well, if not slightly better than the Logistical Regression model.

For this reason, I opted to look into optimization and suggest the GaussianNB model on account of meing over twice as fast as the Logistical Regression model while maintaining excellent accuracy and F1 scores.
