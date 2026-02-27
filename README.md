# Used Car Price Analysis

A data science project following the **CRISP-DM framework** to identify the key drivers of used-car prices and build regression models that can support pricing decisions for a used-car dealership.

## Dataset

The dataset is sourced from Kaggle: [Used Cars Dataset](https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data)

1. Download `vehicles.csv` from the link above.
2. Place it in a `data/` subdirectory at the root of this repository:
   ```
   used-car-price-analysis/
   └── data/
       └── vehicles.csv
   ```

## Structure

| Section | Description |
|---|---|
| Business Understanding | Frame the problem as a supervised regression task |
| Data Understanding | Explore distributions, missing values, and feature correlations |
| Data Preparation | Clean data, engineer features, encode categoricals, scale numerics |
| Modeling | Train Linear Regression, Ridge, Lasso, and Random Forest models |
| Evaluation | Compare models via RMSE / MAE / R², analyse residuals, and rank feature importances |
| Deployment | Actionable recommendations for the dealership |

## Running the Notebook

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook prompt_II.ipynb
```

## Key Findings

- **Vehicle age** and **odometer reading** are the strongest predictors of price.
- **Random Forest** outperforms linear models (R² ≈ 0.80+).
- **Pickup trucks, SUVs, and 4WD/AWD** vehicles command price premiums.
- **Newer, low-mileage inventory** from popular brands offers the best return.
