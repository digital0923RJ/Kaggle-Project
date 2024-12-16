# Data-Science---Kaggle-Project
List of things that i personally have been particiated in several compeition of the Kaggle to improve my understanding in Data Science. 
Here I like to share projects that i was been involoved with. Each compeition brought me a great joy and lessons learned. I do not want to forget and take it as granted. 

## [Classification with an Academic Success Dataset]
- ### Overview
This project aims to predict academic success using a classification model based on a given dataset. Various machine learning techniques and ensemble methods were applied to improve prediction accuracy and AUC scores.

- ### Methodology 
Data Preprocessing
1. Encoding: Categorical target variables were encoded using LabelEncoder.
2. Feature Scaling: Input features were scaled using StandardScaler to standardize the data for improved model performance.

Exploratory Data Analysis
1. Confusion Matrices: confusion matrices for multiple models (XGB, CB, LGBM, HGB, GB, RF, and Ensemble. The models perform very well for the Graduate and Dropout classes but struggle with the Enrolled class, which is consistently misclassified. The Ensemble model balances performance effectively and appears to be a robust choice overall.
2. Boxplot: 
   2.1 Shows the distribution of accuracies for each model across folds, highlighting variance and potential outliers.
   2.2 Displays fold-wise AUC distributions, allowing you to assess the variance and reliability of AUC scores for each model. 
3. Barplot: 
   3.1 Compares average accuracies, providing a clear overview of each model’s performance 
   3.2 Compares the average AUC scores for all models, making it easy to identify the best-performing model.
4. ROC Curve Visualization: To evaluate the performance of classification models by plotting the trade-off between True Positive Rate (TPR) and False Positive Rate (FPR). The ensemble model demonstrates a slight advantage by having consistently high ROC curves across all classes

Models Used
1. Logistic Regression
2. Random Forest
3. XGBoost
4. LightGBM
5. CatBoost

Cross-Validation
1. Stratified K-Fold: Ensured balanced class distribution across folds.
2. Evaluated models using accuracy and AUC metrics for each fold.

Hyperparameter Tuning: Hyperparameters for each model were optimized using Optuna to enhance performance.

Ensemble Learning
1. Predictions from all models were combined using equal weights to create an ensemble.
2. Ensemble predictions were evaluated for overall accuracy and AUC.

- ### Results
1. Performance Metrics: Individual model accuracies and AUCs were logged for comparison.
2. Final ensemble accuracy and AUC scores were computed as follows: Accuracy ()  / AUC () 


## Exploring Mental Health Data
- ### Overview: 
This project focuses on analyzing and predicting mental health outcomes based on survey data. The primary goal is to implement classification models to predict outcomes and identify important factors influencing mental health.
- ### Methodology 
Data Preprocessing
1. Missing values are handled by replacing them with 'missing'.
2. LabelEncoder is used to encode categorical data into numerical values.
3. Data is standardized using StandardScaler for consistent scaling.

Exploratory Data Analysis
1. Correlation Matrix: Used seaborn and dython to calculate correlation coefficients between categorical and continuous variables, visualized with a heatmap.
2. Sunburst Chart: Utilized plotly to create a Sunburst chart that shows hierarchical data distribution. Visualizes the distribution of Gender and Age in a nested structure.

Models Used: Hyperparameter optimization is performed using Optuna.
1. Logistic Regression
2. Random Forest
3. XGBoost
4. LightGBM
5. CatBoost

Cross-Validation
1. Stratified K-Fold: Used a 5-fold cross-validation strategy to maintain balanced class distributions. Evaluated each model using accuracy and AUC metrics for each fold.

Ensemble Learning 
1. Combined predictions from multiple models using equal weights for an ensemble approach.
2. Final predictions achieved improved accuracy and robustness.

- ### Results
1. Performance Metrics: Individual model accuracies and AUCs were logged for comparison.
2. Final ensemble accuracy and AUC scores were computed as follows: Accuracy ()  / AUC ()


## Regression with a Flood Prediction Dataset
- Goal: 
- Approach: Ensamble. 
- why? 1) 
2) 
3) 