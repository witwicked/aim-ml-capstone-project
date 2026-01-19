# AIM ML Capstone Project – Credit Card Fraud Detection

## Overview
This project presents an end-to-end machine learning pipeline for detecting fraudulent credit card transactions using the ULB Credit Card Fraud Dataset.  
The objective is to balance fraud detection effectiveness with operational efficiency, focusing on recall, precision, and interpretability.

Two presentations accompany this project:
- **Technical Deck** – methodology, modeling, metrics, explainability
- **Business Deck** – ROI, risks, and strategic recommendations for executives

---

## Project Structure
```
.
├── decks/
│ ├── de-Guzman_Abigail_Capstone-Project_Business-Deck-compressed.pdf
│ └── de-Guzman_Abigail_Capstone-Project_Technical-Deck-compressed.pdf
├── notebooks/
│ ├── de_Guzman_Abigail_Capstone_Project.ipynb
│ └── de-Guzman_Abigail_Capstone-Project-Notebook.pdf
├── README.md
├── requirements.txt
└── LICENSE
```

---

## Dataset
- **Source**: ULB Credit Card Fraud Dataset  
  https://www.kaggle.com/datasets/waqasishaq/credit-card-fraud-dataset
- The dataset is not stored in this repository due to size and licensing constraints.
- File used: `creditcard.csv`

---

## Models Implemented
- **Logistic Regression** (baseline, class-weighted)
- **Random Forest** (constrained complexity, class-weighted)

Evaluation emphasized:
- ROC-AUC
- Fraud Recall
- Fraud Precision
- False Positive reduction

---

## Model Explainability
SHAP (SHapley Additive exPlanations) was used to:
- Identify key drivers of fraud predictions
- Support transparency and auditability
- Reduce over-reliance on transaction amount

---

## Key Outcomes
- Random Forest outperformed Logistic Regression in fraud precision
- Fewer false positives → reduced manual review costs
- Model explainability supports regulatory and business trust

---

## How to Reproduce
1. Download `creditcard.csv` from Kaggle
2. Install dependencies:
```bash
pip install -r requirements.txt
