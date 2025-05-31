# 💳 Loan Default Prediction — Machine Learning Project

This project builds and evaluates machine learning models to **predict whether a loan applicant will default or not**, based on financial and demographic data. It aims to support smarter lending decisions and risk management for financial institutions.

---

## 🎯 Project Objective

In the financial sector, identifying potential loan defaulters is critical to minimizing losses. The objective of this project is to:
- Develop classification models to predict loan defaults
- Understand key features contributing to credit risk
- Provide strategic business recommendations for lenders

---

## 🗃️ Dataset Overview

- **Source**: Bajaj Finserv
- **Records**: 5,000
- **Features**: 17 (including loan type, credit score, interest rate, employment type)
- **Target**: `default_status` (binary: 0 = No Default, 1 = Default)

---

## 🔧 Data Preparation

- Dropped ID and date columns
- Handled missing values (median/mode)
- Label Encoding for categorical variables
- StandardScaler for numerical features

---

## 📊 Exploratory Data Analysis (Key Findings)

-  Majority of customers were non-defaulters
-  Higher credit scores correlated with fewer defaults
-  High-interest loans were more likely to default
-  Certain employment types showed elevated risk

---

## 🤖 Models Built

| Model | Why Chosen |
|-------|------------|
| **Logistic Regression** | Simple, interpretable baseline |
| **Random Forest** | Handles non-linear patterns and overfitting well |
| **Support Vector Machine (SVM)** | Performs well with high-dimensional, scaled data |

---

## 📉 Model Evaluation

- All models achieved ~80% accuracy but **failed to predict defaulters** due to class imbalance.
- Precision/Recall for default cases was **0.00** across models.
- Next steps: Apply **SMOTE**, adjust **class weights**, or try **XGBoost** with balanced settings.

---

## 📌 Feature Importance

| Logistic Regression | Random Forest |
|---------------------|----------------|
| ↑ Gender, Interest Rate (positive risk factors) | ↑ Loan Amount, Interest Rate, Credit Score |
| ↓ Credit Score, Loan Type (protective) | ↓ Loan Term, Education Level |

---

## 💼 Business Recommendations

- **Raise credit score cut-offs** for approval
- **Monitor high-interest loans** more closely
- **Flag risky employment types** (e.g., gig workers)
- **Prioritize secured loan types**
- **Use longer loan terms** for borderline risk profiles

---

## 🧪 Tech Stack

- Python, Pandas, Scikit-learn
- Jupyter Notebook
- Matplotlib, Seaborn

---

## 📫 Contact

**Ibrahim Fahd Bindawod**  
 
📧 ibrahim.bindawod@gmail.com

---

> “Credit scoring isn’t just about prediction — it’s about protecting people, portfolios, and potential.”
