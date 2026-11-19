# Problem Set 4: The Model That Fit Too Well

ECON 3916 · Applied Data Analytics

A simulated panel of 400 stores is used to reproduce a revenue model with in-sample R² 0.94, diagnose why it fails, and build a better one.

- The original model fits a straight line where revenue flattens with floor area, so it over-forecasts the largest stores by about $2.6M on average.
- Adding a squared floor-area term gives an expected error of about $1.84M RMSE per store (nested 5-fold CV).
- The departing analyst's "validated" R² came from selecting features on all rows before cross-validation; with pure-noise predictors it reports 0.10 against −0.325 when done correctly.

