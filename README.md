# Project Name: Autism Spectrum Disorder Prediction

## Overview:
This project aims to predict Autism Spectrum Disorder (ASD) using machine learning techniques. The dataset used for this project was collected from Kaggle and initially uploaded as `Raw_data.csv`. After initial preprocessing, which includes AQ10 score calculation, a new dataset was created and saved as `New_data.csv`. Further preprocessing steps were undertaken before model training.

## Dataset:
- **Original Dataset**: `Raw_data.csv` from Kaggle
- **Preprocessed Dataset**: `New_data.csv` (After AQ10 score calculation)

## Preprocessing Steps:
1. **AQ10 Score Calculation**: Investigated through Autism Spectrum Disorder criteria, where AQ10 score above 4 for toddlers and above 7 for others indicates autism. Calculated and replaced AQ10 scores in the dataset.
2. **Further Preprocessing**:
   - Removed unnecessary features.
   - Replaced categorical values with numerical binary values.
   - Conducted data standardization for improved model performance.

## Modeling:
- **Models Used**: AdaBoost and Support Vector Machine (SVM)
- **Model Evaluation**:
  - AdaBoost:
    - Achieved 100% accuracy in both training and testing.
    - Due to potential overfitting, this model was discarded.
  - SVM:
    - Achieved 89.3% accuracy in training.
    - Achieved 89.5% accuracy in testing.

## Prediction:
Utilized the trained SVM model to make predictions on new datasets.

## Files:
1. `Raw_data.csv`: Original dataset collected from Kaggle.
2. `New_data.csv`: Dataset after AQ10 score calculation.
3. `Preprocessed_data.csv`: Fully preprocessed dataset ready for model training.
4. `svm_model.pkl`: Pickled SVM model for future predictions.
