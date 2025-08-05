# Autism Spectrum Disorder (ASD) Prediction

This project uses machine learning models to predict the presence of Autism Spectrum Disorder based on clinical and behavioral features.

## Dataset
- Source: [Kaggle - Autism Diagnosis](https://www.kaggle.com/competitions/autismdiagnosis/overview)
- Only the `train.csv` was used for model development.

## Models Used
- Decision Tree
- Random Forest
- XGBoost

## Preprocessing
- SMOTE was applied to handle class imbalance.
- Standard data cleaning and encoding were performed.

## Evaluation Metrics
- **Recall**: Prioritized to reduce false negatives, critical in ASD detection.
- **F1-Score**: Balanced metric considering both false positives and false negatives.
- **Accuracy**: Used to assess overall model performance.

## Best Model
- **Random Forest Classifier**
  - `max_depth=10`, `n_estimators=500`, `min_samples_leaf=2`, `bootstrap=False`
  - Achieved **92% cross-validation accuracy**

## Why Random Forest?
- Robust to noise and outliers
- Handles non-linear relationships
- Works well with high-dimensional data
- Feature importance aids explainability
- Balanced performance and efficiency


