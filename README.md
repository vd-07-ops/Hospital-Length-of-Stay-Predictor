# Hospital-Length-of-Stay-Predictor (Fundamentals of Machine Learning Assignment 1)
This project has been made using 4 different types of regression models (Linear Regression, Random Forest Regressor, Decision Tree Regressor, Gradient Boosting Regressor).
This project will be helpful to hospital to allocate the resources according to patients' conditions and giving them an estimate of how much each patient will be using up hospital's resources.

## Team Name: The Predictive Squad

## Team Members:

1. Kashish Patel - 202418044
2. Vedant Dave - 202418014
3. Sujal Dhrangdhariya - 202418017
4. Jatin Sindhi - 202418055

# Project Documentation
## 1. Data Preparation & Processing :-
### Loading Data :
**->** Read health data from CSV files scrapped from DataSet Link given below. A complete description of dataset is given in the link below

DataSet Link :
https://microsoft.github.io/r-server-hospital-length-of-stay/input_data.html

## 2. Feature Engineering :-
**->** Drop Columns eid, vdate, discharged, facid

**->** Assigning Value for gender column (F = 1 & M = 0)

**->** As in rcount column we have values like 5+ so we replaced them with 5.

## 3. Visualization :-
1. Box plot for length of stay :-
2. Correlation Matrix of our feature with our target variable
3. readmission count vs length of stay (Scatter Plot)
4. Medical condition vs. average length of stay (bar plot)
5. All medical report values vs. length of stay (bar plot)

## 4. Training / Testing / Splitting :-
1. Splitting Our data in 80:10:10 (Train Data : Validation Data : Test Data)
2. Merging train and validation set together for further model training

## 5. Model Training :-
### 1. Linear Regression Model:

  **Psuedocode**:
  1. Fit the model on train set.
  2. Model will predict the value using test set.
  3. Find errors using difference of predicted set and test set.
  

### 2. Random Forest Regressor

  **Psuedocode**:

  1. Initialize model's hyperparameters (eg. n_estimators=100)
  2. Fit the model on training set.
  3. Predict the output of model using test set.
  4. Find error values using different metrics.

### 3. Decision Tree Regressor

  **Psuedocode**:
  
  1. Instantiate the model class.
  2. Fit the model on training set.
  3. Predict the outcome of model using test set.
  4. Find error values using different metrics.


### 4. Gradient Boosting Regressor

  **Psuedocode**:
  1. Instantiate the model class and initialize the hyperparameters (eg. n_estimators=100, learning_rate=0.8, max_depth=3).
  2. Fit the model on training set.
  3. Predict the outcome of model using test set.
  4. Find error values using different metrics.
     
## 6. Model Pipeline:-
      Data Loading -> Data Preprocessing -> Split Data -> Model Selection -> Model Training -> Model Evaluation -> Model Prediction

## 7. Contributions/Novelty:-

This predictor model will not only help hospital personnel but also the insurance providers who can get an estimate of how long a patient will be living in the hospital based on his/her medical conditions this will help them settle the claim amount accordingly and there will be less chances of fradulent cases as previously patients used to show higher no. of days just to claim a higher amount from the insurance providers.

Hospitals will be benefitted by this model in a way that they can easily manage and allocate resources for each patient if they get a rough estimate of patient's stay.

## 8. Citations:-


*   For Dataset: https://microsoft.github.io/r-server-hospital-length-of-stay/

*   For Regression Model: https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html

* For Random Forest Regressor: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html

* For Decision Tree Regressor: https://scikit-learn.org/stable/auto_examples/tree/plot_tree_regression.html

* For Gradient Boosting Regressor: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingRegressor.html




