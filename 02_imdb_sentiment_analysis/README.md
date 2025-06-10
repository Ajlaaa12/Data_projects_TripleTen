# IMDB Sentiment Analysis

**Goal**: Classify IMDB movie reviews as positive or negative.

**Tools & Techniques**:
- NLTK and spaCy for text preprocessing
- TF-IDF vectorization
- Logistic Regression, LGBMClassifier

**Key Steps**:
- Tokenized and cleaned review data
- Handled class balance
- Trained and compared multiple models
- Tried BERT on a small subset (excluded due to performance)

**Final Model & Metric**:
- Logistic Regression (F1 = 0.89)

**Conclusion**:
The model met and exceeded the F1 target of 0.85. NLTK + TF-IDF + Logistic Regression is the best choice for speed and accuracy.

### Future Improvements
- Fix model limitations with sarcasm and complex sentiment using transformer-based models (e.g., BERT) to achieve deeper contextual understanding.
- Improve classification robustness using ensemble methods (e.g., blending Logistic Regression with LGBM).
- Enhance UX by deploying a Streamlit app to let users input custom reviews and get instant predictions.****
