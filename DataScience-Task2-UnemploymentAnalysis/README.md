# DataScience-Task2-UnemploymentAnalysis

## Objective
Exploratory Data Analysis (EDA) on unemployment data in India, focused on uncovering regional and temporal trends and the impact of the COVID-19 pandemic on unemployment rates.

## Dataset
State-wise monthly unemployment statistics for India (Jan 2020 – Oct 2020):
- `Region` — Indian state
- `Date` — observation month
- `Frequency` — reporting frequency (Monthly)
- `Estimated Unemployment Rate (%)`
- `Estimated Employed`
- `Estimated Labour Participation Rate (%)`
- `Zone` — broader geographic zone (South/North/East/West/etc.)
- `longitude`, `latitude`

Source: publicly available "Unemployment in India" dataset (originally sourced from CMIE, redistributed widely for data science coursework).

## Tech Stack
Python, pandas, matplotlib, seaborn, Jupyter Notebook

## What's in this notebook
- Data loading, shape/dtype inspection, null check
- Region-wise and month-wise average unemployment analysis
- Time-series line chart across major states
- Top 10 states by highest average unemployment rate
- Correlation heatmap (unemployment rate vs. employment vs. labour participation)
- Pre-COVID vs. post-COVID comparison (split at India's 25 March 2020 lockdown date)
- Zone-wise comparison as an additional non-obvious insight
- Written markdown observations after every chart
- Conclusion with 3 actionable takeaways

## How to run
```
pip install pandas matplotlib seaborn jupyter
jupyter notebook unemployment_analysis.ipynb
```

## Files
- `unemployment_analysis.ipynb` — full analysis notebook (pre-executed with outputs)
- `unemployment.csv` — dataset used
