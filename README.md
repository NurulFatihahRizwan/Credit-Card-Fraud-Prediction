# 💳 Credit Card Fraud Detection

A streamlined machine learning project to predict fraudulent credit card transactions using **Python** and **Scikit-Learn**. 

## Project Overview
The goal of this project is to build a binary classifier that distinguishes between legitimate transactions and fraudulent ones. Since fraud cases are rare (only **0.17%** of the data), this project focuses on optimizing **Precision** and **Recall** rather than simple Accuracy.

## Dataset Specifications
* **Source:** Kaggle Credit Card Fraud Detection Dataset
* **Total Records:** 284,807
* **Features:** `Time`, `Amount`, and 28 anonymized PCA-transformed features (`V1` – `V28`).
* **Target:** `Class` (0: Not Fraud, 1: Fraud)

## Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib

## Model Performance
The model was evaluated using a `classification_report` to ensure fraudulent cases were captured effectively.

### Results:
| Metric | Class 0 (Legit) | Class 1 (Fraud) |
| :--- | :--- | :--- |
| **Precision** | 1.00 | 0.84 |
| **Recall** | 1.00 | 0.69 |
| **F1-Score** | 1.00 | 0.76 |

> **Note:** The Precision of **0.84** indicates that when the model flags fraud, it is correct 84% of the time. The Recall of **0.69** shows we are successfully catching 69% of all actual fraud cases.



## Key Learnings
* **Class Imbalance:** Learned how to evaluate models when one class significantly outweighs the other.
* **Metric Selection:** Identified why Recall is the "North Star" metric for financial security projects.
* **Data Scaling:** Handled PCA-transformed features to maintain model performance.

## Future Roadmap
- [ ] Implement **SMOTE** (Synthetic Minority Over-sampling Technique) to improve Recall.
- [ ] Compare performance against **Random Forest** and **XGBoost**.
- [ ] Perform hyperparameter tuning to reduce false negatives.
