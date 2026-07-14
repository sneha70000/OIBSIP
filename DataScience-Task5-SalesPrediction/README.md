Internship: OASIS INFOBYTE, Summer Internship Program (SIP)  
Track: Data Science  
Task: Task 5 · Sales Prediction Using Python  

Objective  
Create a regression model to predict product sales based on advertising spending across three media channels: TV, Radio, and Newspaper.  

Dataset  
The classic Advertising.csv dataset, with 200 rows, is a well-known public dataset from An Introduction to Statistical Learning by James, Witten, Hastie, and Tibshirani. It teaches linear regression. The columns are as follows:  

Column  Description  
TV       Advertising spending on TV (in $ thousands)  
Radio    Advertising spending on Radio (in $ thousands)  
Newspaper Advertising spending on Newspaper (in $ thousands)  
Sales    Product sales (in thousands of units)  

Tech Stack  
Python 3  
pandas, numpy  
scikit-learn (LinearRegression, RandomForestRegressor, train_test_split, metrics)  
matplotlib, seaborn  
Jupyter Notebook  

What the Notebook Covers  
Data loading and exploratory data analysis including null check, descriptive statistics, and a pairplot of all features.  
Individual scatter plots for Sales versus TV, Radio, and Newspaper spending.  
Correlation matrix heatmap.  
Train/test split with an 80/20 ratio.  
Baseline Linear Regression model.  
Additional Random Forest Regressor model.  
Model evaluation including MAE, RMSE, and R² score for both models, presented in a comparison table.  
Residual plot for the best-performing model.  
Interpretation of coefficient analysis for Linear Regression and feature importance for Random Forest to identify the advertising channel that impacts Sales the most.  
Conclusion with a business takeaway.  

Key Finding  
TV advertising spending is the strongest predictor of Sales, followed by Radio. Newspaper spending contributes the least explanatory power, which is consistent across both the correlation analysis and the trained models.  

Files in This Folder  
Sales_Prediction.ipynb - full, executed, commented Jupyter Notebook  
Advertising.csv - source dataset  
README.md - this file  

How to Run  
pip install pandas numpy scikit-learn matplotlib seaborn jupyter  
jupyter notebook Sales_Prediction.ipynb  

Self-Sourcing Note  
The dataset comes from the classic public "Advertising.csv" dataset (TV, Radio, Newspaper leading to Sales), commonly found on Kaggle and various educational GitHub repositories.