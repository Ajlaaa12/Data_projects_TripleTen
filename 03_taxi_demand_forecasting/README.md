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

### Future Improvements
- Fix prediction noise during peak hours using more granular lag features and hybrid models.
- Improve performance using Prophet or LSTM for time series with irregular seasonality.
- Integrate live weather and flight data using APIs to improve short-term forecasting accuracy.
