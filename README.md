# Real Estate Price Prediction: Feature Scaling

Predicts **house price per unit area** and compares how feature scaling affects different regression models.

## Tech
Python, Pandas, Scikit-learn, Matplotlib

## Models compared
Linear Regression (with and without Min-Max / Robust scaling), Random Forest, Gradient Boosting, and SVR (with and without scaling). Metrics: R², cross-validated R², MAE, RMSE.

## Key points
- Scalers are inside pipelines, so they are fitted on training data only (no data leakage).
- The row-number column `No` is dropped because it is not a real feature.
- Scaling does not change Linear Regression results, but it matters for SVR.

## Data
Add `Real estate.csv` (Real Estate Valuation dataset, columns X1 to X6 and Y) next to `ml/scaling/scaling.ipynb`.

## Run it
```
pip install pandas numpy scikit-learn matplotlib jupyter
jupyter notebook ml/scaling/scaling.ipynb
```
