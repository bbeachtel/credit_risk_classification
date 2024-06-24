### Loan Risk Prediction Analysis
## Project Overview
This project develops predictive models to assess loan risk using financial data, classifying loans as high-risk (1) or healthy (0). The dataset includes features like loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

## Installation
Ensure Python and the following libraries are installed: pandas, scikit-learn, lazypredict.

## Data
The dataset should be in CSV format with relevant financial columns and an encoded target variable, loan_status. It should be located in the 'Resources' directory.

## Preprocessing
Steps include:
    - Loading the dataset into a Pandas DataFrame.
    - Defining 'loan_status' as the target and other columns as features.
    - Splitting the data into training and testing sets using train_test_split.
    - Modeling with a Logistic Regression model to establish a baseline.
    - Use LazyClassifier to benchmark various other models quickly.
    - Evaluate models using accuracy, precision, and recall scores with a confusion matrix and classification report.

## Results
## Key findings:

## Logistic Regression: High accuracy (0.99), precision (0.86), and recall (0.93).
## GaussianNB: Similar accuracy, excellent precision, and recall, and significantly faster than Logistic Regression.
## Recommendation: 
The GaussianNB model is recommended for its speed and excellent performance, making it suitable for scenarios requiring rapid loan risk assessment.

## Summary
This project provides an effective approach to predicting loan risk. The GaussianNB model stands out for its efficiency and high performance. For detailed implementation, refer to the project files.