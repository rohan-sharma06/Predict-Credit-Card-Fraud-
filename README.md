# 🛡️ Credit Card Fraud Detection

This project aims to **develop a machine learning classification model** that detects fraudulent transactions based on patterns in:

- 💰 Transaction Amount  
- 🌍 Location  
- 📱 Device Usage  
- 👤 User Behavior

## 📌 Problem Statement

**Goal:** Build a model that accurately identifies fraudulent credit card transactions.  
This is a binary classification task where the model learns to distinguish between legitimate and fraudulent activities.

## 🔍 Dataset

The dataset contains anonymized credit card transactions with features such as time, amount, and PCA-transformed values for privacy. The key column is:

- `Class`: 0 → Legitimate | 1 → Fraudulent

> **Note:** The dataset is highly imbalanced, with fraud being a small minority.

## 🧠 Approach

1. **Data Preprocessing**
   - Handle class imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**
   - Split into training and testing sets
   - Normalize features using **StandardScaler**

2. **Model Training**
   - Use **Random Forest Classifier** for its robustness and interpretability

3. **Evaluation**
   - Accuracy
   - Classification Report (Precision, Recall, F1-Score)
   - ROC AUC Score
   - Confusion Matrix
   - ROC Curve

## 📦 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
