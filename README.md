# Credit Card Fraud Detection

## Overview
Analysis of 284,807 real credit card transactions to identify fraudulent behavior patterns and build a predictive model. The dataset is highly imbalanced — only 0.17% of transactions are fraudulent.

## Key Findings

**Behavioral patterns:**
- 50% of fraud transactions involve amounts under $10 — consistent with card testing behavior before larger theft
- Fraud peaks at 2AM (57 cases) and 11AM (53 cases)
- The highest-value fraud occurs at midnight, with an average transaction of $303 — nearly 2.5x the overall fraud average

**Model performance:**

| Model | Precision | Recall |
|---|---|---|
| Logistic Regression | 0.85 | 0.58 |
| Random Forest | 0.97 | 0.77 |

Random Forest significantly outperforms Logistic Regression. For fraud detection, Recall is the critical metric — a missed fraudster is more costly than a false alarm. The final model achieves AUC = 0.95.

## Project Structure
```
fraud_detection/
├── analysis.ipynb       ← EDA, SQL analysis, model training
└── README.md
```

## Tools Used
Python · Pandas · Matplotlib · Seaborn · SQLite · scikit-learn

## Dataset
[Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)