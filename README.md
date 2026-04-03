# Store-Classification-using-Machine-Learning-
Project Overview

This project focuses on classifying 124 retail stores into three performance categories—'Low', 'Moderate', and 'High'—based on historical transaction data. The analysis involves extensive data cleaning, feature engineering, and a comparative study of various machine learning algorithms.

Key Objectives

Data Preprocessing: Cleaned a dataset of 473,974 records, addressing missing values (7.58% in item descriptions) and correcting data entry errors in item prices using mode-based imputation.
Feature Engineering: Developed performance metrics for each store, including:
  TotalSalesSum: Product of item price and quantity sold.
  Customer Metrics: Unique customer counts and sales per customer.
  Efficiency Metrics: Sales per transaction and sales per square foot of shop area.
Exploratory Data Analysis (EDA): Identified right-skewed distributions and high multicollinearity between variables like transaction counts and total sales.

Machine Learning Models

The project evaluated several classification models using GridSearchCV for hyperparameter tuning:
  Tree-based Models: Decision Trees, Random Forest, Extra Trees, XGBoost, AdaBoost, and LightGBM.
  Linear Models: Logistic Regression with Lasso (L1) and Ridge (L2) regularization.
  Ensemble Methods: StackingClassifier.

Results & Conclusion

  Best Performing Model: Lasso Logistic Regression emerged as the superior model, achieving an accuracy of 0.71 and a weighted F1-score     of 0.70.
  Key Insight: Linear models outperformed complex tree-based models (like Random Forest), which suffered from overfitting despite           regularization.
  Feature Importance: Lasso regularization identified TotalSalesSum, TotalQuantitySold, and UniqueCustomers as the most significant         predictors of store performance.
