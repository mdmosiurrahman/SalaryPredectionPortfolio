# Salary Predection Portfolio
Salary Prediction Project(Python)

## Define the problem
 Salary is always the vital indicator for job seeker to start the career. It's also important for employer. It is one of the difficult tasks for employer/HR to offer ideal salary to ideal candidate not only saves the budget for the company but also not overlook the talents of the candidates
## Project Goal
The goal of this project is to examine the dataset of job postings, and predict salaries for a new set of postings which involves building a model to predict the salaries given in the test dataset.
## Practical Use
HR Department who need real-time solutions in order to make effective employment offers to potential hires.
## Tool
Python 3 (Jupyter Notebook) with a wide range of libraries/packages available for data manipulation and predictive modeling algorithms.

## Data
train_features.csv: Each row represents metadata for an individual job posting. The job Id column represents a unique identifier for the job posting. The remaining columns describe features of the job posting.

train_salaries.csv: Each row associates a job Id along with salary.

test_features.csv: Similar to train_features.csv, each row represents metadata for an individual job posting.

## Features
* Job-Type - Janitor, Manager, CEO, CFO etc.
* Degree - High school, College, Master's etc.
* Major - Physics, Biology, Maths etc.
* Industry - Health, Finance, Oil etc.
* Years-of_Experience - Candidate experience in years
* Miles-From_Metropolis - Distance from the Metropolis

Every row has a unique JOB-ID, there is a column and COMPANY-ID which is the company identifier.

## Data Discovery Steps
1.Import Libraries and set up directory where python interpreter access code files
2.Load Data
3.Examine and Get Insights on Data
4.The 3 input files each have 1 million rows.
  * Merged train data (train_features + train_target) which has 1 million rows and 9 columns
  * Test Feature data has 1 million rows and 8 columns
  * Datasets have mixed data types (categorical and numeric)
5.Clean data  
  * No duplicates in data
  * Datasets do not have null values
  * Check for invalid data - Dropped 5 rows of data with invalid Salary (salary less than or equal to 0)
6.Explore data
7.Summarize Numerical and Categorical variables. Confirmed jobId is a unique identifier for the job postings
8.Review Correlation between each feature and the target variable using plots and feature counts as required
9.Identify correlation between all features respectively by using label encoding categorical features with the mean salary
10.Set baseline model
   * Using the correlation martix, identified the highest correlated feature and use this to build a simple linear regression model to predict the salary, using negative mean squared error as the quality of an estimator and values closer to zero are better
   * The baseline MSE error was 1367
11. Hypothesize solutions
   * Multiple Linear Regression - includes more than one feature, which could improve the model
   * Random Forest Regressor - improves the accuracy by reducing overfitting problem and the variance in decision trees
   * GradientBoostingRegressor - data contains weakly correlated features, gradient boosting regression combines weak learners into a single strong learner, which          could be an improvement to the baseline model
   
## Feature Summary

## Correlation Matrix

## Model Development

## Deploy Solution


