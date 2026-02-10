# Indian Sign Language Recognition (ISL)

This repository contains a **comparative study of classical machine learning models and a Convolutional Neural Network (CNN)** for **Indian Sign Language (ISL) alphabet recognition**, developed as part of the *Machine Learning Using Python* course.

## Datasets Used

Two publicly available Kaggle datasets were used:

1. **Large ISL Dataset**  
   - Classes: 1–9, A–Z  
   - Total samples: 42,745  
   - Observation: Images per class were highly similar with identical backgrounds, leading to near-duplicate samples.

2. **Small Realistic ISL Dataset**  
   - Classes: A–Z (excluding H, J, Y)  
   - Total samples: 702  
   - Observation: Fewer samples per class but higher diversity in background, lighting, skin tone, and hand pose.

## Models Implemented

- Logistic Regression (HOG features)
- Linear SVM (SGD-based)
- Random Forest
- Convolutional Neural Network (CNN)

## Key Findings

- Extremely high accuracies on the large dataset were caused by **low data diversity and near-duplicate images**, not true generalization.
- On the smaller, more realistic dataset:
  - Classical models performed better than CNNs.
  - CNN accuracy was low due to insufficient training data.
- This study highlights that **dataset quality and diversity matter more than raw accuracy**.

## Conclusion

High accuracy alone is not a reliable indicator of model performance. Proper dataset analysis and realistic evaluation are essential, especially for computer vision tasks like sign language recognition.

## Repository Contents

- `ISL_Model_Comparison.ipynb` — complete implementation and experiments
- Model comparison plots and confusion matrices (generated within the notebook)
