# Age Verification with Computer Vision

**Goal**: Predict the age of a person from a facial photo to help supermarkets comply with alcohol sales regulations.

**Tools & Techniques**:
- ResNet50 (transfer learning)
- ImageDataGenerator (rescale, augmentation)
- TensorFlow, Keras
- GPU training (Google Colab)

**Key Steps**:
- Performed EDA on facial age distribution
- Augmented and preprocessed image data
- Trained and fine-tuned ResNet50 with dropout layers

**Final Model & Metric**:
- MAE = 6.53 on validation set (goal was ≤ 8)

**Conclusion**:
The model performs well on unseen data and can be deployed as part of an automated checkout age verification system.
