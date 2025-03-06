# Credit Card Fraud Detection - CodSoft Data Science Internship

## Project Overview
This project focuses on detecting fraudulent credit card transactions using **Logistic Regression** and **Random Forest Classifier**. Given the imbalanced nature of fraud detection, **SMOTE (Synthetic Minority Over-sampling Technique)** is applied to balance the dataset.

## Dataset Information
The dataset used in this project is **creditcard.csv**, sourced from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). It contains anonymized transaction details:
- **Time** - Seconds elapsed between the transaction and the first transaction in the dataset.
- **V1-V28** - Principal components obtained from PCA (anonymized transaction features).
- **Amount** - Transaction amount.
- **Class** - Transaction label (0: Non-Fraudulent, 1: Fraudulent).

## Data Preprocessing & Exploration
- **Class Distribution Analysis** - Checking class imbalance.
- **Transaction Amount Analysis** - Visualizing fraud vs. non-fraud amounts.
- **Feature Analysis** - Boxplots and histograms for fraud vs. non-fraud transactions.
- **Scaling Features** - Standardizing features using **StandardScaler**.
- **Handling Imbalance** - Using **SMOTE** to oversample fraudulent transactions.

## Model Training
- **Algorithms Used**:
  - Logistic Regression
  - Random Forest Classifier
- **Data Splitting**: 80% Training, 20% Testing
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - Confusion Matrix

## Model Performance
### Logistic Regression:
- **Accuracy:** 97.41%
- **Precision:** 5.79%
- **Recall:** 91.83%
- **F1 Score:** 10.89%

### Random Forest:
- **Accuracy:** 99.95%
- **Precision:** 87.10%
- **Recall:** 82.65%
- **F1 Score:** 84.82%

**Key Observations:**
- Logistic Regression has high recall but low precision, leading to false positives.
- Random Forest achieves a better balance with high accuracy and F1-score.

## How to Run the Project
1. Install required libraries:
   ```sh
   pip install pandas numpy seaborn scikit-learn imbalanced-learn matplotlib
   ```
2. Place the dataset file (`creditcard.csv`) in the same directory as the script.
3. Run the Python script to train models and evaluate fraud detection.
4. Visualizations and performance metrics will be displayed.

## Future Improvements
- Hyperparameter tuning for better fraud detection.
- Exploring advanced models like **XGBoost, LightGBM, and Neural Networks**.
- Implementing real-time fraud detection with an API.

## Author
- **CodSoft Data Science Internship** - Credit Card Fraud Detection Project
