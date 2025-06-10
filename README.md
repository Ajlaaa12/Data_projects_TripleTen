# Data_projects_TripleTen

This repository contains selected data science and machine learning projects I completed as part of the TripleTen bootcamp. Each project solves a real-world business challenge using data-driven techniques.

---

## Table of Contents

1. [Age Verification with Computer Vision](#1-age-verification-with-computer-vision)
2. [IMDB Sentiment Analysis](#2-imdb-sentiment-analysis)
3. [Sweet Lift Taxi Demand Forecasting](#3-sweet-lift-taxi-demand-forecasting)
4. [Insurance Benefit Prediction & Privacy](#4-insurance-benefit-prediction--privacy)

---

## 1. Age Verification with Computer Vision
**Goal**: Build and evaluate a model to estimate a person’s age from a facial photograph to help Good Seed supermarket comply with alcohol sales laws.  
**Metric**: MAE ≤ 8  
**Best Model**: ResNet50-based CNN (MAE = 6.53)  
**Techniques**: EDA, ImageDataGenerator, ResNet50 with GlobalAveragePooling & Dropout, trained on GPU.  
**Conclusion**: The ResNet50 model surpassed the benchmark with MAE = 6.53. It generalized well across age groups, especially near critical legal thresholds like 18 years.

---

## 2. IMDB Sentiment Analysis
**Goal**: Classify IMDB movie reviews as positive or negative.  
**Metric**: F1 Score ≥ 0.85  
**Best Model**: NLTK + TF-IDF + Logistic Regression (F1 = 0.89)  
**Other Models**: spaCy + TF-IDF + Logistic Regression (F1 = 0.88), spaCy + LGBM (F1 = 0.83)  
**Exclusion**: BERT was tested on a small subset but excluded due to performance issues.  
**Conclusion**: NLTK-based preprocessing with TF-IDF and Logistic Regression yielded the best results. The model met the F1 score requirement and maintained strong generalization.

---

## 3. Sweet Lift Taxi Demand Forecasting
**Goal**: Predict the number of taxi orders for the next hour.  
**Metric**: RMSE ≤ 48  
**Best Model**: Tuned CatBoost (RMSE = 43.12)  
**Other Strong Models**: LightGBM (RMSE = 43.26), Random Forest (RMSE = 46.08), SARIMA (RMSE = 47.67)  
**Techniques**: Time series decomposition, lag features, rolling means, SARIMA, ensemble models with hyperparameter tuning.  
**Conclusion**: CatBoost was the top-performing model, generalizing well across time with minimal error.

---

## 4. Insurance Benefit Prediction & Privacy
**Goal**: Solve four ML tasks for Sure Tomorrow Insurance:  
1. **Customer Similarity**: PCA + kNN revealed patterns in income/age/family size; scaling was essential for clustering.  
2. **Eligibility Classification**: Scaled kNN reached F1 = 0.943, outperforming dummy models even under class imbalance.  
3. **Benefit Count Prediction**: Linear regression with and without scaling achieved RMSE = 0.36; age was the top predictor.  
4. **Privacy-Preserving Obfuscation**: Feature matrix transformation using invertible matrix P retained exact model performance post-obfuscation.  
**Conclusion**: Machine learning supports marketing, eligibility prediction, and secure data transformation. Model performance was preserved even after applying obfuscation, ensuring ethical AI practices.

---

### 📬 Contact  
Feel free to reach out or explore more of my work:  
**📧** aa.mutapcic@gmail.com | [**LinkedIn**](www.linkedin.com/in/ajla-mutapcic)
