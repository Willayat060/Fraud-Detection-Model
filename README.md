# Fraud-Detection-Model
Machine Learning-based Fraud Detection System using Logistic Regression and XGBoost on a financial transactions dataset (~6.3M records). Developed as part of an INSAID Data Science Internship challenge to proactively identify fraudulent activity using real-world transaction patterns.

# 💳 Fraud Detection in Financial Transactions

This project demonstrates a machine learning pipeline to detect fraudulent financial transactions using supervised classification algorithms, built as part of an internship task at INSAID (International School of AI & Data Science).

---

## 📁 Dataset

- **Size:** ~6.3 million records
- **Columns:** 11
- **Target Variable:** `isFraud` (1 = Fraud, 0 = Normal)
- **Data Source:** Provided for internship purpose by INSAID
- **Key Features:**
  - Transaction step, type, amount
  - Account balances before and after transactions
  - Flags indicating fraudulent behavior

---

## 📌 Objectives

- Clean and preprocess a large-scale dataset
- Handle class imbalance in fraud classification
- Build, train, and compare classification models
- Evaluate models using metrics suited to imbalanced datasets
- Identify important predictors of fraud
- Recommend actionable fraud prevention strategies

---

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- XGBoost

---

## 🤖 Models Used

| Model                | AUC Score | Notes |
|---------------------|-----------|-------|
| Logistic Regression | 0.97      | Strong baseline |
| XGBoost             | 1.00      | Final selected model |

---

## 🔍 Key Insights

- `newbalanceOrig`, `oldbalanceOrg`, `amount`, and `transaction type` are the top fraud indicators
- Fraudulent transactions are typically high-value withdrawals leaving origin accounts nearly empty
- Class imbalance handled using `scale_pos_weight` and `class_weight=balanced`

---

## 📊 Evaluation Metrics

- ROC-AUC Curve
- Confusion Matrix
- Precision, Recall, F1-Score
- Feature Importance (XGBoost)

---

## 🧠 Business Recommendations

- Limit unverified large TRANSFER/CASH_OUT actions
- Introduce anomaly-based transaction monitoring
- Use behavior profiling and multi-factor authentication
- Deploy real-time fraud scoring using models like XGBoost

---

## 📂 Files in This Repository

| File | Description |
|------|-------------|
| `Fraud_Detection_Model_INSAID.ipynb` | Full notebook: data cleaning, modeling, evaluation |
| `README.md` | This documentation |
| `fraud.csv` | *[Dataset not included due to size/licensing]* |

---

## 🧑‍💻 Author

**Willayat Hussain**  
Final year Computer Science student | Machine Learning & Data Science Enthusiast  
GitHub: [Willayat060](https://github.com/Willayat060)

---

## 📬 Contact

For any queries or collaboration, feel free to reach out via GitHub or LinkedIn.

