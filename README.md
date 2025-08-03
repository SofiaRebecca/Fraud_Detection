# 💸 Fraud Detection Using XGBoost

This project is a machine learning solution to detect **fraudulent transactions** in a financial dataset of over 6 million records. The goal was to proactively identify fraud while minimizing false alarms.

---

## 🚀 Project Summary

- **Model Used**: XGBoost Classifier
- **Focus**: Only `TRANSFER` and `CASH_OUT` transactions (where all fraud occurs)
- **Key Features Engineered**:
  - `errorBalanceOrig`: mismatch in original balance
  - `errorBalanceDest`: unexpected jump in destination balance
- **Imbalance Handling**: `scale_pos_weight` used instead of SMOTE

---

## 📊 Final Model Performance

| Metric          | Value       |
|-----------------|-------------|
| Accuracy        | 99.9%       |
| Recall (Fraud)  | 100%        |
| Precision (Fraud) | 83%       |
| F1-score (Fraud) | 91%        |

> ✅ Catches all fraud cases  
> ⚠️ Minimal false positives  
> 🎯 Excellent fraud detection model for production-like systems

---

## 🧠 How It Works

1. **Filter Data** for only fraud-prone transaction types
2. **Feature Engineering** to extract suspicious behaviors
3. **Handle Imbalance** using XGBoost’s `scale_pos_weight`
4. **Train & Tune** model with clean evaluation
5. **Threshold Tuning & ROC/PR Analysis** (optional)

---

## 📁 Files Included

- `Fraud_Detection_Project_Sofia.ipynb` — full Jupyter Notebook with step-by-step code and insights
- `Data Dictionary.txt` — explanation of each column
- `Task Details.pdf` — internship task brief

---

## 👩‍💻 Author

**Sofia Rebecca**  

---

## ✅ Future Work

- Use SHAP for explainability
- Integrate into real-time fraud pipeline
- Deploy with a Flask/Django REST API

---

## 📢 Notes

This project was built for the **Accredian Internship Task** using real-world ML workflows and practices. It's suitable for showcasing in your resume or portfolio.
