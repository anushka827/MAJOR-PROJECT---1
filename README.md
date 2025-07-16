# MAJOR-PROJECT---1
# Credit Card Fraud Detection

This project implements a **Credit Card Fraud Detection system** using **Machine Learning** on the **Kaggle Credit Card Fraud Detection dataset**.

## 📂 Dataset

- Source: [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Transactions made by European cardholders in September 2013.
- Highly **imbalanced dataset** with only 0.17% fraud cases.
- Features are anonymized PCA components (`V1`, `V2`, ..., `V28`) plus `Time` and `Amount`.

---

## 🛠️ Project Pipeline

✅ **1. Data Loading & Preprocessing**
- Handled missing values.
- Analyzed class distribution.
- Feature-label separation (`X`, `y`).

✅ **2. Handling Imbalanced Data**
- Used **SMOTE (Synthetic Minority Over-sampling Technique)** to balance fraud vs non-fraud samples.

✅ **3. Model Training**
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

✅ **4. Evaluation**
- Accuracy
- Classification report
- Confusion Matrix visualization

✅ **5. Model Saving**
- Saved the best-performing model (`credit_card_fraud_model.pkl`) for deployment or further usage.

---

## 📊 Results

Using **XGBoost with SMOTE**, achieved:

- **High recall on fraud class**, ensuring detection of fraudulent transactions.
- Balanced accuracy across classes despite dataset imbalance.
- Clear visualization with a confusion matrix for evaluation.

---

## 🚀 How to Run

1️⃣ Open the notebook in [Google Colab](https://colab.research.google.com).  
2️⃣ Upload the Kaggle `creditcard.csv` dataset or use Kaggle API for direct download.  
3️⃣ Run cells step-by-step:
   - Data preprocessing
   - SMOTE balancing
   - Model training
   - Evaluation
   - Model saving
   - Confusion matrix visualization
4️⃣ Download your trained `credit_card_fraud_model.pkl` for deployment.

---

## 📌 Requirements

- Python
- pandas, numpy
- scikit-learn
- imblearn
- xgboost
- matplotlib, seaborn

All dependencies can be installed in Colab or locally using:

```bash
pip install pandas numpy scikit-learn imbalanced-learn xgboost matplotlib seaborn
