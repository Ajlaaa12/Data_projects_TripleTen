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


### Future Improvements
- Fix prediction accuracy near the legal threshold age (18) using a custom loss function to penalize misclassifications more in that range.
- Improve generalization by adding more diverse training images using facial augmentation tools.
- Speed up inference using a lighter CNN model (e.g., MobileNet) to deploy in real-time on edge devices.
