# 💳 Credit Card Fraud Detection using Machine Learning

---

## 📌 Project Overview

### Objective
Build an end-to-end machine learning system to detect fraudulent credit card transactions.

- **Domain:** Finance / Risk Analytics  
- **Target Variable:** `Class`  
  - 0 → Legitimate transaction  
  - 1 → Fraudulent transaction  

### Key Challenges
- Highly imbalanced dataset (~0.17% fraud cases)  
- Minimize false negatives (missed fraud)  
- Minimize false positives (customer inconvenience)  

---

## 1️⃣ Define the Problem Clearly

### 🔹 Problem Statement
Credit card fraud causes significant financial loss and customer distrust. The goal is to detect fraud accurately and early, minimizing false negatives.

### 🔹 ML Task
- **Problem Type:** Binary Classification  
- **Classes:** Fraud (1) vs Non-Fraud (0)  
- **Challenge:** Extreme class imbalance  

### 🎯 Business Objective
Build a model to classify transactions, prioritizing **high recall** and **ROC-AUC** due to extreme imbalance.

---

## 2️⃣ Data Collection

### 📂 Dataset Source
- Public Kaggle Credit Card Fraud Dataset  
- Transactions from European cardholders  

### 📊 Dataset Features
- 284,807 transactions  
- 30 numerical features (PCA-transformed V1–V28)  
- `Time`, `Amount`  
- Target: `Class`  

---

## 3️⃣ Data Cleaning & Preprocessing

### 🔹 Analyzing the Data
- Check dataset shape, info, and summary statistics  

### 🔹 Missing Values
- Dataset contains **no missing values**  

### 🔹 Duplicates
- Remove duplicate rows  

### 🔹 Target Distribution
```text
0 → Normal transactions
1 → Fraud transactions
