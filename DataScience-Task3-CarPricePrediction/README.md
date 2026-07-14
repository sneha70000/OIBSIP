# DataScience-Task3-CarPricePrediction

## Objective
Build a regression model that predicts the selling price of a used car based on features such as brand, age, mileage, fuel type, and transmission.

## Dataset
301 used car listings with:
- `Car_Name` — model name
- `Year` — manufacture year
- `Selling_Price` — target variable (resale price, in lakhs INR)
- `Present_Price` — original ex-showroom price
- `Kms_Driven` — kilometers driven
- `Fuel_Type` — Petrol / Diesel / CNG
- `Seller_Type` — Dealer / Individual
- `Transmission` — Manual / Automatic
- `Owner` — number of previous owners

Source: the widely-used "car data.csv" (CarDekho used-vehicle dataset), commonly hosted on Kaggle and GitHub for ML coursework.

## Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook

## What's in this notebook
- Data cleaning: duplicate removal, categorical consistency check
- Feature engineering: `Car_Age` derived from year, `Brand` extracted from car name
- EDA: selling price distribution, price vs. fuel type, price vs. car age
- One-hot encoding of categorical variables
- Feature correlation heatmap
- 80/20 train/test split
- 3 regression models trained: Linear Regression, Random Forest Regressor, Gradient Boosting Regressor
- Evaluation via MAE, RMSE, R² for every model
- Feature importance chart for the best-performing model

## How to run
```
pip install pandas numpy scikit-learn matplotlib seaborn notebook
jupyter notebook car_price_prediction.ipynb
```
Then: **Kernel → Restart & Run All**

## Files
- `car_price_prediction.ipynb` — full analysis notebook (pre-executed with outputs)
- `car_data.csv` — dataset used
