# Financial Market Analysis

This project explores historical financial market data with Python. The notebook analyzes price trends and growth, examines relationships between assets, and builds a linear regression model to estimate S&P 500 closing prices.

## Project Files

- `Final_Project.ipynb` - Data exploration, visualizations, regression, asset clustering, and PCA.
- `financial_regression.csv` - Main dataset used by the notebook.

## Dataset Source

The `financial_regression.csv` dataset is from [Gold Price Regression by franciscogcc on Kaggle](https://www.kaggle.com/datasets/franciscogcc/financial-data). It contains time-series financial data for market indices, commodities, economic indicators, and foreign exchange rates from 2010 to 2024. The Kaggle dataset page states that the data was obtained from Alpha Vantage and FRED APIs and is licensed under [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).

## Analyses

- Cleans and inspects financial time-series data, including missing values and duplicate rows.
- Visualizes closing prices and growth from 2010 to 2024 for the S&P 500, Nasdaq, gold, silver, oil, platinum, and palladium.
- Compares asset closing prices with a correlation heatmap and groups assets using K-means clustering.
- Uses PCA to visualize the asset clusters in two dimensions.
- Predicts S&P 500 closing prices from open, high, low, and volume values using linear regression and time-series cross-validation. Model metrics include MAE, MSE, RMSE, and R².

## Requirements

Python 3 and Jupyter Notebook or JupyterLab are required. Install the notebook dependencies with:

```bash
python -m pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Run

1. Clone or download this repository.
2. Install the requirements above.
3. Start Jupyter from the project directory:

   ```bash
   jupyter notebook
   ```

4. Open `Final_Project.ipynb` and run its cells in order. Keep `financial_regression.csv` in the same directory as the notebook.

## Optional SPY Data

The notebook also contains a section that reads `Download Data - FUND_US_ARCX_SPY.csv` to evaluate predictions against a separate SPY dataset. That file is not included in this project. To run that section, provide the CSV in the project directory with the columns expected by the notebook (`Date`, `Open`, `High`, `Low`, `Volume`, and `Close`).