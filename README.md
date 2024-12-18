# Loan Repayment Prediction Using-Decision Tree and Random Forest-Models

## Objective
This project aims to predict whether borrowers will fully repay their loans using machine learning techniques. The dataset, sourced from Lending Club (2007-2010), provides valuable borrower and loan details. The primary goal is to create accurate classification models to assist investors in evaluating loan risk.

## Dataset Features
The dataset contains the following features:
- credit.policy: Indicates whether the customer meets Lending Club's credit criteria (1 = Yes, 0 = No).
- not.fully.paid: Indicates whether the customer has fully paid off their debt or not (1 = Not fully paid, 0 = Debt has been fully paid)
- purpose: Purpose of the loan (e.g., "credit_card", "debt_consolidation").
- int.rate: Loan interest rate as a proportion (e.g., 0.11 for 11%).
- installment: Monthly loan installment.
- log.annual.inc: Log-transformed annual income of the borrower.
- dti: Debt-to-income ratio.
- fico: Borrower’s FICO credit score.
- days.with.cr.line: Number of days the borrower has had a credit line.
- revol.bal: Borrower’s revolving balance.
- revol.util: Borrower’s revolving line utilization rate.
- inq.last.6mths: Number of creditor inquiries in the last 6 months.
- delinq.2yrs: Number of delinquencies in the last 2 years.
- pub.rec: Number of derogatory public records.

## Methodology
#### 1. Data Cleaning
  Removed missing values from the dataset.
  Encoded categorical variables using one-hot encoding.
#### 2. Exploratory Data Analysis (EDA)
  Visualized feature distributions and relationships using histograms, boxplots, and heatmaps.
  Analyzed the correlation between features to understand their influence on loan repayment.
#### 3. Data Preprocessing
  Separated the target variable (not.fully.paid) from the features.
  Split the dataset into training and testing sets (70% training, 30% testing).
#### 4. Model Development
  Decision Tree: Built a Decision Tree Classifier and visualized its structure.
  Random Forest: Trained a Random Forest Classifier for improved accuracy and robustness.
#### 5. Evaluation Metrics
**Classification Report**:  Evaluated precision, recall, and F1-score.  
**Confusion Matrix**:  Assessed model performance on true positives, false positives, true negatives, and false negatives.  
**Feature Importance Analysis**:  Identified key features influencing loan repayment, such as installment, days.with.cr.line, and revol.util.

## Key Results
Decision Tree Performance:
- Precision: 75%, Recall: 73%, F1-Score: 74%.
- Correctly predicted loan repayment 2002 times but misclassified 429 loans as unpaid and 339 as paid incorrectly.
Random Forest Performance:
- Precision: 80%, Recall: 85%, F1-Score: 78%.
- Correctly predicted loan repayment 2421 times with only 10 false negatives but 432 false positives.

## Tools and Libraries
**Python Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn.  
**Machine Learning Concepts**: Decision Tree, Random Forest, Feature Importance, Model Evaluation (Precision, Recall, F1-Score, Confusion Matrix).


