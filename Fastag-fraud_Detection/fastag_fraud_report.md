
# 🚧 Fastag Fraud Detection: Bullet Point Report

## 📌 Objective
- Detect fraudulent FASTag transactions using toll and vehicle-related data.

---

## 📁 Dataset Overview
- 5000 transactions, 13 features.
- Key columns:
  - `Transaction_ID`, `Timestamp`
  - `Vehicle_Type`, `FastagID`, `TollBoothID`
  - `Transaction_Amount`, `Amount_paid`
  - `Vehicle_Speed`, `Geographical_Location`
  - `Fraud_indicator` (Target label)

---

## 🧹 Data Preprocessing
- Loaded data from Google Drive.
- Used Pandas to inspect data (`head()`, `shape`).
- Identified missing values (e.g., in `FastagID`).
- Checked data types and basic statistics.

---

## 📊 Exploratory Data Analysis (EDA)
- Analyzed class distribution of `Fraud_indicator`.
- Explored mismatch between `Transaction_Amount` and `Amount_paid`.
- Compared vehicle types and fraud rates.
- Reviewed tollbooth patterns and speed anomalies.
- Used plots to visualize trends (bar plots, histograms, box plots).

---

## 🤖 Modeling *(if included in your notebook)*
- Categorical encoding of features.
- Train-test split.
- Applied classification models (e.g., Logistic Regression, Random Forest).
- Evaluated metrics: Accuracy, Precision, Recall, F1-score.

---

## ✅ Key Insights
- Fraud often involves underpayment or zero payment.
- Some vehicle types (e.g., large or commercial) are more fraud-prone.
- Certain toll booths report more fraud.
- Missing `FastagID` is often linked to fraud.

---

## 🛠 Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook / Google Colab
- CSV data source from Google Drive

---

## 📌 Recommendations
- Flag transactions with payment mismatch in real-time.
- Monitor high-fraud tollbooths more strictly.
- Mandate valid Fastag registration before processing tolls.
