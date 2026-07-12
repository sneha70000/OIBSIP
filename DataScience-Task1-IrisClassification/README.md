# DataScience-Task1-IrisClassification

## Objective
Train and evaluate machine learning classification models to identify the species of an iris flower (*Setosa*, *Versicolor*, or *Virginica*) from its physical measurements.

## Dataset
The classic Iris dataset, loaded directly from `sklearn.datasets.load_iris()` — no external download required. 150 samples, 4 numeric features (sepal length, sepal width, petal length, petal width), 3 balanced classes (50 samples each).

## Tech Stack
Python, scikit-learn, pandas, matplotlib, seaborn, Jupyter Notebook

## What's in this notebook
- Exploratory Data Analysis: shape, dtypes, null check, descriptive statistics, class balance
- Visualisations: seaborn pairplot, per-feature box plots by species, correlation heatmap
- Feature selection discussion: identifies petal length & petal width as the most discriminative features
- 80/20 stratified train/test split with feature scaling
- 4 classifiers trained: Logistic Regression, K-Nearest Neighbours, Decision Tree, Random Forest
- Evaluation: accuracy, confusion matrices, full classification reports (precision/recall/F1) for every model
- Best-model selection with data-driven justification

## Results Summary
All four models achieve strong accuracy (typically 90–100% on the test set) since the Iris classes are close to linearly separable, especially on petal measurements. See the notebook for the exact accuracy achieved by each model on this run and the declared best performer.

## How to run
```
pip install pandas numpy scikit-learn matplotlib seaborn notebook
jupyter notebook iris_classification.ipynb
```
Then: **Kernel → Restart & Run All**

## Files
- `iris_classification.ipynb` — full analysis notebook (pre-executed with outputs)
