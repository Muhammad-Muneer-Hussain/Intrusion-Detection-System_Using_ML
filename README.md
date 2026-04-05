# Intrusion Detection System Using Machine Learning  

**Author:** Muhammad Muneer Hussain  
**Date:** 12 November 2025  
**Semester Project:** Information Security – 5th Semester, BS IT  
**Dataset:** KDDTrain++.csv (Network Intrusion Detection Dataset, 125,972 records, 43 features)  

---

## Project Overview
This project was completed as part of my **semester Information Security course**. The goal was to develop a **Machine Learning-based Intrusion Detection System (IDS)** to classify network traffic as **Normal** or **Attack**.  

---

## 1️⃣ Dataset Selection & Problem Framing
- **Dataset:** KDDTrain++.csv  
- **Problem Type:** Binary Classification  
- **Goal:** Detect whether a network connection is **Normal** or **Attack** based on network behavior.  

---

## 2️⃣ Data Preprocessing & Feature Engineering
- Checked dataset structure, null values, and duplicates (none found).  
- Converted all non-normal outcomes to `attack` for binary classification.  
- Applied **RobustScaler** to scale numeric features.  
- Encoded categorical columns (`protocol_type`, `service`, `flag`) using **one-hot encoding**.  
- Reduced features from 122 → 20 using **PCA** for efficiency.  
- Split dataset into **80% training** and **20% testing** sets.  

---

## 3️⃣ Machine Learning Models & Evaluation

### Models Used
- Logistic Regression  
- Support Vector Machine (Linear SVC)  
- Decision Tree Classifier  

### Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- Confusion Matrix  

| Model | Train Accuracy | Test Accuracy | Precision | Recall |  
|-------|----------------|---------------|-----------|-------|  
| Logistic Regression | 88.70% | 88.52% | 85.21% | 91.37% |  
| Support Vector Machine | 97.20% | 97.04% | 97.64% | 96.01% |  
| Decision Tree Classifier | 99.99% | 99.85% | 99.84% | 99.84% |  

**✅ Best Model:** Decision Tree Classifier (**Test Accuracy: 99.85%**)  

---

## 4️⃣ Sample Predictions  

| Row | Prediction |  
|-----|-----------|  
| 1 | Normal ✅ |  
| 2 | Attack 🚨 |  
| 3 | Normal ✅ |  

---

## 5️⃣ Conclusion
- The IDS was successfully developed using **ML techniques**.  
- Decision Tree Classifier achieved the highest performance and effectively detected malicious traffic.  
- This model demonstrates potential for **real-time intrusion detection applications**.  

---

## 6️⃣ Technologies & Libraries Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn (Logistic Regression, SVM, Decision Tree, PCA, metrics)  

---

## 7️⃣ How to Run / Usage
1. Clone the repository:  
```bash
git clone https://github.com/Muhammad-Muneer-Hussain/repo-name.git
