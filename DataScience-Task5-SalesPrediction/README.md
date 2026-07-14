# Data Science, Task 5: Sales Prediction Using Python

**Internship:** OASIS INFOBYTE, Summer Internship Program (SIP)  
**Track:** Data Science  
**Task:** Task 5 · Sales Prediction Using Python  

## Objective  
Create a regression model to predict product sales based on advertising spending across three media channels: **TV**, **Radio**, and **Newspaper**.  

## Dataset  
The classic `Advertising.csv` dataset (200 rows) is a well-known public dataset from *An Introduction to Statistical Learning* (James, Witten, Hastie, Tibshirani). It is used to teach linear regression. Columns:  

| Column     | Description                                   |  
|------------|------------------------------------------------|  
| TV         | Advertising spending on TV (in $ thousands)       |  
| Radio      | Advertising spending on Radio (in $ thousands)    |  
| Newspaper  | Advertising spending on Newspaper (in $ thousands)|  
| Sales      | Product sales (in thousands of units)          |  

## Tech Stack  
- Python 3  
- pandas, numpy  
- scikit-learn (LinearRegression, RandomForestRegressor, train_test_split, metrics)  
- matplotlib, seaborn  
- Jupyter Notebook  

## What the Notebook Covers  
1. Data loading and exploratory data analysis (null check, descriptive statistics, pairplot of all features)  
2. Individual scatter plots: Sales vs. TV, Radio, and Newspaper spending  
3. Correlation matrix heatmap  
4. Train/test split (80/20)  
5. Baseline Linear Regression model  
6. Additional Random Forest Regressor model  
7. Model evaluation: MAE, RMSE, R² score for both models, in a comparison table  
8. Residual plot for the best-performing model  
9. Interpretation: coefficient analysis (Linear Regression) and feature importance (Random Forest) to identify which advertising channel has the biggest impact on Sales  
10. Conclusion with a business takeaway  

## Key Finding  
TV advertising spending is the strongest predictor of Sales, followed by Radio. Newspaper spending contributes the least explanatory power, which is consistent across both the correlation analysis and the trained models.  

## Files in This Folder  
- `Sales_Prediction.ipynb` — full, executed, commented Jupyter Notebook  
- `Advertising.csv` — source dataset  
- `README.md` — this file  

## How to Run  
```bash  
pip install pandas numpy scikit-learn matplotlib seaborn jupyter  
jupyter notebook Sales_Prediction.ipynb  
```  

## Self-Sourcing Note  
The dataset is sourced from the classic public "Advertising.csv" dataset (TV, Radio, Newspaper → Sales), commonly found on Kaggle and various educational GitHub repositories.