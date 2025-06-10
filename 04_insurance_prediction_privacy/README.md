# Insurance Benefit Prediction & Privacy

**Goal**: Help an insurance company improve decisions using ML for:
- Customer similarity
- Benefit eligibility classification
- Benefit count regression
- Privacy-preserving data transformation

**Tools & Techniques**:
- PCA, kNN, Euclidean/Manhattan distances
- Logistic Regression, Dummy classifiers
- Custom Linear Regression
- Matrix-based data obfuscation

**Key Steps**:
- Scaled features and applied kNN to find similar customers
- Used scaled kNN for classification (F1 = 0.943)
- Built linear regression for benefit count
- Applied invertible matrix to obfuscate features and proved it didn't affect predictions

**Final Model & Metrics**:
- Classification: kNN F1 = 0.943
- Regression: RMSE = 0.36, R² ≈ 0.66

**Conclusion**:
ML models can significantly improve targeting, eligibility prediction, and protect sensitive customer data with zero impact on model performance.

### Future Improvements
- Fix limitations in benefit count prediction using tree-based regressors (e.g., XGBoost) for better nonlinearity capture.
- Improve similarity detection with clustering algorithms like DBSCAN or HDBSCAN.
- Enhance security by testing other obfuscation methods like differential privacy or federated learning.
