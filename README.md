# ML_IT4060_Assignment
A group assginment

# 📊 Telco Customer Churn Prediction (ML Project)

This project aims to predict customer churn in the telecommunications industry using supervised machine learning techniques. It uses real-world data from the [Telco Customer Churn dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) to build predictive models that help businesses identify at-risk customers and take proactive retention measures.

---

## 🚀 Project Overview

**Objective:**  
To predict whether a customer will churn (leave the company) using historical customer data.

**Dataset:**  
- Source: Kaggle  
- Records: 7,043 customers  
- Features: Demographic data, account info, service subscriptions, and payment details  
- Target: `Churn` (Yes / No)

---

## 🧠 Machine Learning Models Used

We applied and compared the performance of three supervised learning algorithms:

1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Support Vector Machine (SVM)**

### ✅ Model Enhancements
- **Hyperparameter Tuning** using `GridSearchCV`
- **Cross-Validation** (5-fold) to ensure stability
- **SMOTE** (Synthetic Minority Over-sampling Technique) to address class imbalance
- **Feature Importance** analysis for business insight
- **Correlation Heatmap** for multicollinearity detection

---

## 📈 Results Summary

| Model                | Accuracy | Recall (Churn) | F1-Score (Churn) |
|----------------------|----------|----------------|------------------|
| Logistic Regression  | 82.3%    | 60%            | 0.64             |
| Random Forest        | 80.4%    | 50%            | 0.57             |
| SVM (Tuned)          | 81.6%    | 52%            | 0.60             |
| Logistic + SMOTE     | 80.0%    | 82%            | 0.81             |
| RF + SMOTE           | 82.3%    | 86%            | 0.83             |
| SVM + SMOTE          | 78.9%    | 82%            | 0.80             |

---

## 📁 Project Structure

```
├── ML-assignment.ipynb          # Jupyter Notebook with code
├── report.pdf                   # Final report (main deliverable)
├── submission.txt               # Dataset, GitHub, and YouTube links
├── members.txt                  # Team member details
└── README.md                    # This file
```

---

## 👥 Team Members

- [Shangeeth V] — Random Forest + Grid Search + Feature Analysis
- [Sanjeeva N] — Support Vector Machine + Kernel Tuning
- [Asmitha T] — Logistic Regression + SMOTE

---

## 🎥 Project Demo

Watch our video presentation here:  
[👉 YouTube Video](https://youtu.be/your-video-id)

---

## 📊 Dataset

This project uses the publicly available **Telco Customer Churn dataset** from Kaggle:  
🔗 [https://www.kaggle.com/datasets/blastchar/telco-customer-churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## 📌 Requirements

- Python 3.x
- pandas, numpy, seaborn, matplotlib
- scikit-learn
- imbalanced-learn

Install dependencies:
```bash
pip install -r requirements.txt
```

---

## 💡 Future Work

- Deploy the model via a Flask API or Streamlit dashboard
- Add more customer behavioral data (e.g., call logs, support tickets)
- Explore Gradient Boosting and XGBoost models
