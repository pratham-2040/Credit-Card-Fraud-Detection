# Credit Card Fraud Detection  
### Financial Risk Analytics | Comparative Machine Learning Study

---

## Project Overview

This project presents a systematic comparative study of supervised machine learning models for detecting fraudulent credit card transactions. The objective is to evaluate model performance under highly imbalanced financial data conditions and identify the most effective approach for real-world fraud detection systems.

The study compares Logistic Regression, Random Forest, Gradient Boosting, and XGBoost using a consistent preprocessing and evaluation framework.

---

## Problem Statement

Credit card fraud detection is challenging due to:

- Severe class imbalance (fraudulent transactions represent less than 0.2% of total data)
- Overlapping transaction behavior patterns
- High business cost of false negatives (missed fraud cases)

Traditional accuracy metrics are insufficient in such scenarios. Therefore, this project emphasizes precision, recall, F1-score, ROC-AUC, and confusion matrix analysis for proper performance evaluation.

---

## Dataset

- Dataset: Credit Card Fraud Detection Dataset (Kaggle)
- Total Transactions: 284,807
- Fraudulent Transactions: 492
- Features: 30 anonymized PCA-transformed features
- Target Variable: Fraud (1) / Legitimate (0)

The dataset is highly imbalanced and reflects real-world financial transaction challenges.

---

## Methodology

### Data Preprocessing
- Stratified train-test split to preserve class distribution
- Feature-target separation
- SMOTE (Synthetic Minority Oversampling Technique) applied to training data only

### Model Development
The following supervised models were trained and evaluated:

- Logistic Regression
- Random Forest
- Gradient Boosting
- XGBoost

Each model was tested on:
- Original imbalanced dataset
- SMOTE-balanced dataset

---

## Evaluation Metrics

To properly assess fraud detection performance, the following metrics were used:

- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

These metrics provide a balanced view of fraud detection effectiveness beyond simple accuracy.

---

## Comparative Insights

### Logistic Regression
- Interpretable baseline model
- Struggles with complex, non-linear fraud patterns
- Lower recall under imbalanced conditions

### Random Forest
- Captures non-linear feature interactions
- Improved fraud detection performance
- Moderate computational cost

### Gradient Boosting
- Sequential error correction improves detection
- Performs well with balanced data
- Requires careful tuning

### XGBoost
- Best overall performance
- Highest recall and ROC-AUC
- Strong capability in handling imbalanced datasets
- Suitable for high-risk financial environments

---

## Key Findings

- Class imbalance significantly impacts fraud detection accuracy.
- SMOTE improves recall across all models.
- Ensemble-based models outperform linear models.
- XGBoost provides the most reliable and consistent results.

---

## Proposed Framework

Comparative Fraud Detection Framework (CFDF):

1. Load dataset
2. Perform stratified split
3. Apply SMOTE to training data
4. Train multiple supervised models
5. Evaluate using advanced metrics
6. Compare results and generate insights

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Matplotlib / Seaborn

---

## Practical Implications

- Logistic Regression can serve as a lightweight first-stage filter.
- Ensemble models are better suited for complex fraud detection tasks.
- XGBoost is recommended for high-risk transaction evaluation.
- Imbalance-aware training techniques are essential in financial systems.

---

## Future Improvements

- Cost-sensitive learning integration
- Two-stage fraud detection architecture
- Real-time fraud detection systems
- Feature selection with imbalance-aware optimization

---

## Author

Prathmesh Tiwari  
