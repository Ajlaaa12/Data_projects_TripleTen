# Sweet Lift Taxi Demand Forecasting

**Goal**: Forecast hourly taxi demand to help the company attract drivers during peak hours.

**Tools & Techniques**:
- Time Series Analysis (trend, seasonality)
- SARIMA model
- CatBoost, LightGBM, Random Forest
- Feature engineering (lags, rolling means)

**Key Steps**:
- Resampled and visualized time series data
- Created lag-based features
- Tuned models using TimeSeriesSplit cross-validation

**Final Model & Metric**:
- CatBoost (RMSE = 43.12), meets RMSE ≤ 48 goal

**Conclusion**:
Tuned CatBoost outperformed other models and generalized well across the data. SARIMA was also a strong traditional baseline.
