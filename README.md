# Decision Tree Regression on Insurance Dataset

## Overview

This project applies a Decision Tree Regressor to the popular `insurance.csv` dataset to predict medical insurance charges based on demographic and lifestyle features. The project demonstrates end to end machine learning steps including data preprocessing, model training, evaluation, feature importance analysis, and visualization.

## Dataset

The dataset contains the following columns

* age
* sex
* bmi
* children
* smoker
* region
* charges (target variable)

## Steps Performed

### 1. Data Preparation

* Loaded the dataset using Pandas
* Transformed categorical features (sex, smoker, region) into numerical values using Label Encoding
* Defined `charges` as the target variable and all other features as predictors
* Split the data into training and test sets with an 80 to 20 ratio

### 2. Model Training

* Implemented `DecisionTreeRegressor` from Scikit Learn
* Trained the model on the dataset to capture relationships between features and the target

### 3. Evaluation

* Evaluated the model using the R² score on both training and test sets
* Compared results to understand performance and generalization

### 4. Feature Importance

* Extracted feature importance values from the trained model
* Identified smoking status, age, and body mass index as the most significant predictors of insurance charges

### 5. Visualization

* Bar chart to show feature importance
* Decision tree visualization using `plot_tree` for interpretability

## Key Insights

* Smoking status is the strongest predictor of high insurance charges
* Age and body mass index are also highly influential factors
* Decision Trees provide interpretability which is important for healthcare and insurance applications
* Although prone to overfitting, Decision Trees serve as a solid baseline before moving to ensemble methods such as Random Forests or Gradient Boosting

## Tools and Libraries

* Python
* Pandas
* Matplotlib
* Seaborn
* Scikit Learn

## How to Run

1. Clone the repository
2. Install required Python libraries

   pip install pandas matplotlib seaborn scikit-learn

3. Place `insurance.csv` in the project directory
4. Run the Python script to train and evaluate the model

