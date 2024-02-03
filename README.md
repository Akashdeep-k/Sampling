# Fraud Detection using Credit Card Transactions

## Overview

The project implements the following:

- **Sampling Techniques:**
  - Random Sampling
  - Stratified Sampling
  - Under-sampling
  - Over-sampling
  - SMOTE (Synthetic Minority Over-sampling Technique)

- **Models:**
  - CatBoost
  - XGBoost
  - LightGBM
  - Support Vector Classifier (SVC)
  - Random Forest

## Dataset

The dataset (`credit_card_data.csv`) contains credit card transactions with various features, including transaction amount and timestamp. Handling imbalanced classes is crucial due to the rarity of fraudulent transactions.

## Usage

1. **Data Loading:**
   - Load the credit card dataset from `credit_card_data.csv`.
   - Gain insights into the dataset's structure and features.

2. **Data Preprocessing:**
   - Address any missing values.
   - Investigate and visualize the class distribution to comprehend data imbalance.

3. **Sampling:**
   - Implement five distinct sampling techniques to generate diverse datasets.
   - Ensure equilibrium between fraudulent and legitimate transactions in the sampled datasets.

4. **Model Training:**
   - Train models including CatBoost, XGBoost, LightGBM, SVC, and Random Forest on each sampled dataset.

5. **Model Evaluation:**
   - Assess the accuracy of each model on a dedicated test dataset (not utilized during training).
   - Contrast the performance of models trained with different sampling techniques.

6. **Results and Conclusion:**
   - Summarize the observations, contrasting the efficacy of each sampling technique in enhancing model accuracy for credit card fraud detection.

## Results

Provide insights and comparisons on model performances, highlighting the impact of different sampling techniques on fraud detection accuracy.

| Sampling Technique | Model ↓            | Simple Random Sampling | Stratified Sampling | Bootstrap Sampling | Systematic Sampling | Cluster Sampling |
|--------------------|--------------------|------------------------|----------------------|--------------------|----------------------|-------------------|
| Decision Tree      | Accuracy (%)       | 94.16                  | 96.41                | 98.85              | 97.55                | 97.71             |
| Random Forest      | Accuracy (%)       | 96.75                  | 99.67                | 99.84              | 99.35                | 99.67             |
| SVM                | Accuracy (%)       | 88.96                  | 89.87                | 96.07              | 92.64                | 96.08             |
| KNN                | Accuracy (%)       | 78.57                  | 80.72                | 86.91              | 83.31                | 76.47             |
| XGBoost            | Accuracy (%)       | 94.16                  | 98.04                | 99.84              | 98.36                | 98.69             |


## Conclusion

Summarize the overall findings and suggest recommendations for choosing effective sampling techniques in credit card fraud detection.

**Note:**
- Ensure dependencies are installed, preferably using a virtual environment.
- Follow the provided Jupyter notebook for step-by-step execution.
