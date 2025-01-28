# Data Science - Kaggle Projects

List of things that I have personally participated in several competitions on Kaggle to improve my understanding of Data Science.  
Here, I would like to share projects that I have been involved with. Each competition brought me great joy and lessons learned. I do not want to forget them or take them for granted.

---

## [Classification with an Academic Success Dataset]

### Overview
This project aims to predict academic success using a classification model based on a given dataset. Various machine learning techniques and ensemble methods were applied to improve prediction accuracy and AUC scores.

### Methodology 
1. **Data Preprocessing**
   - Encoding: Categorical target variables were encoded using `LabelEncoder`.
   - Feature Scaling: Input features were scaled using `StandardScaler` to standardize the data for improved model performance.

2. **Exploratory Data Analysis**
   - **Confusion Matrices**: Examined confusion matrices for multiple models (XGBoost, CatBoost, LightGBM, HGB, GB, RF, and Ensemble). The models performed well for the Graduate and Dropout classes but struggled with the Enrolled class, which was consistently misclassified. The Ensemble model balanced performance effectively and appeared to be a robust choice overall.
   - **Boxplot**: 
     - Showed the distribution of accuracies for each model across folds, highlighting variance and potential outliers.
     - Displayed fold-wise AUC distributions, assessing the variance and reliability of AUC scores for each model.
   - **Barplot**: 
     - Compared average accuracies, providing a clear overview of each model's performance.
     - Compared the average AUC scores for all models, making it easy to identify the best-performing model.
   - **ROC Curve Visualization**: Evaluated classification model performance by plotting the trade-off between True Positive Rate (TPR) and False Positive Rate (FPR). The ensemble model demonstrated a slight advantage by having consistently high ROC curves across all classes.

3. **Models Used**
   - Ensemble (Logistic Regression, Random Forest, XGBoost, LightGBM, CatBoost)

4. **Cross-Validation**
   - **Stratified K-Fold**: Ensured balanced class distribution across folds.
   - Evaluated models using accuracy and AUC metrics for each fold.

5. **Hyperparameter Tuning**
   - Hyperparameters for each model were optimized using `Optuna` to enhance performance.

### Results
- Performance Metrics: Individual model accuracies and AUCs were logged for comparison.

---

## [Exploring Mental Health Data]

### Overview
This project focuses on analyzing and predicting mental health outcomes based on survey data. The primary goal is to implement classification models to predict outcomes and identify important factors influencing mental health.

### Methodology 
1. **Data Preprocessing**
   - Missing values were handled by replacing them with "missing".
   - Categorical data was encoded into numerical values using `LabelEncoder`.
   - Data was standardized using `StandardScaler` for consistent scaling.

2. **Exploratory Data Analysis**
   - **Correlation Matrix**: Used `seaborn` and `dython` to calculate correlation coefficients between categorical and continuous variables, visualized with a heatmap.
   - **Sunburst Chart**: Utilized `plotly` to create a Sunburst chart showing hierarchical data distribution, including Gender and Age.

3. **Models Used**
   - Logistic Regression
   - Random Forest
   - XGBoost
   - LightGBM
   - CatBoost  
   *Hyperparameter optimization was performed using `Optuna`.*

4. **Cross-Validation**
   - **Stratified K-Fold**: Used 5-fold cross-validation to maintain balanced class distributions. Models were evaluated using accuracy and AUC metrics for each fold.

5. **Ensemble Learning**
   - Combined predictions from multiple models using equal weights for an ensemble approach.
   - Final predictions achieved improved accuracy and robustness.

### Results
- Performance Metrics: Individual model accuracies and AUCs were logged for comparison.

---

## [Regression with a Flood Prediction Dataset]

### Overview
This project aimed to predict the probability of a region flooding based on various factors.

### Methodology 
1. **Data Preprocessing**
   - Included cleaning, handling missing values, and scaling.
2. **Exploratory Data Analysis**
   - Visualized key features and their relationships with the target variable.
3. **Models Used**
   - Applied regression models such as XGBoost, LightGBM, Random Forest, and CatBoost.
4. **Cross-Validation**
   - Used a Stratified K-Fold approach to validate models.
5. **Ensemble Learning**
   - Combined multiple models to improve prediction accuracy and robustness.

### Results
- Models were evaluated based on metrics such as Mean Squared Error (MSE) and R-squared scores.
