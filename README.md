# Class Imbalance Techniques in Machine Learning

## Project Overview

This project explores the impact of different techniques to address class imbalance (CI) on model performance across three diverse datasets. Class imbalance occurs when the distribution of classes is skewed, with one class (minority class) significantly less represented than the other (majority class).

## Objectives

- Implement and compare three different CI techniques
- Evaluate the impact of CI techniques on five classification algorithms
- Analyze performance across three imbalanced datasets

## Datasets

1. Heart Failure Clinical Records Dataset
   Source: Kaggle

2. Stroke Prediction Dataset
   Source: Kaggle

3. Breast Cancer Wisconsin (Diagnostic) Dataset
   Source: UCI Machine Learning Repository
   URL: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data

## CI Techniques Implemented

1. Resampling Method: SMOTE (Synthetic Minority Over-sampling Technique)
2. Algorithmic Method: Class Weighting
3. One-Class Learning: Isolation Forest

## Classification Algorithms

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine (SVM)
5. Naive Bayes

## Methodology

For each dataset:
1. Data Loading and Cleaning
2. Exploratory Data Analysis (EDA)
3. Feature Selection and Data Splitting
4. Applied Standard Scaling to features
5. Implemented baseline models on imbalanced data
6. Applied each CI technique and evaluated performance
7. Compared results across all models and CI techniques

## Performance Metrics

- Precision
- Recall
- F1-Score
- ROC AUC Score

## Key Findings

### Heart Failure Dataset
- Random Forest with SMOTE showed the most significant improvement
- Class Weighting was effective for Random Forest
- Isolation Forest had mixed results across different models

### Stroke Prediction Dataset
- SMOTE generally improved recall for stroke cases across all models
- Random Forest with SMOTE provided the best balance between precision and recall
- Class Weighting in Random Forest did not significantly improve performance
- Isolation Forest had varied results, occasionally enhancing precision for some models

### Breast Cancer Wisconsin Dataset
- SVM with Isolation Forest showed the highest precision and recall for both classes, with an exceptional ROC AUC score
- Random Forest with Class Weighting and Random Forest with SMOTE offered robust performance with improvements in handling class imbalance
- Logistic Regression with SMOTE provided a balanced performance with improved recall for the malignant class
- Isolation Forest technique was particularly effective in improving model performance for this dataset

## Conclusion

- The effectiveness of CI techniques varied across datasets and models
- SMOTE consistently improved recall for minority classes but often at the cost of precision
- Random Forest with SMOTE emerged as a strong performer across multiple datasets
- For the Breast Cancer Wisconsin dataset, SVM with Isolation Forest showed exceptional performance
- The choice of CI technique significantly impacts model performance, highlighting the importance of experimentation in addressing class imbalance

## Repository Structure

- `heart_failure_analysis.py`: Analysis script for Heart Failure dataset
- `stroke_prediction.py`: Analysis script for Stroke Prediction dataset
- `breast_cancer_analysis.py`: Analysis script for Breast Cancer Wisconsin dataset
- `data/`: Directory containing the datasets
- `results/`: Directory containing output visualizations and detailed results
- `README.md`: This file, providing an overview of the project

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- imbalanced-learn

## How to Run

1. Clone this repository
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run each analysis script separately:

## Author
SARAH RAFIQ SHAIKH
