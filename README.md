# 💳 Credit Card Fraud Detection

This project implements various machine learning models to detect fraudulent credit card transactions. Due to the highly imbalanced nature of fraud data, it includes strategies like resampling and metric optimization to ensure robust performance.

## 📁 Project Structure

- `CreditCardFraudDetection.ipynb` – Main notebook containing data analysis, model training, and evaluation.
- `README.md` – Project overview and setup instructions.

---

## 🔍 Problem Statement

Credit card fraud detection is a critical challenge faced by financial institutions. Fraudulent transactions are extremely rare compared to genuine ones, which makes this a **highly imbalanced binary classification problem**. The objective is to identify fraudulent transactions while minimizing false positives and negatives.

---


## 🧠 Models Implemented

- Logistic Regression
- Random Forest
- XGBoost

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Null check, data types, and descriptive stats
   - Feature scaling (StandardScaler for `Amount`)
   - Train-test split with stratification

2. **Handling Imbalance**
   - SMOTE (Synthetic Minority Oversampling Technique)
   - Random undersampling
   - OVERSAMPLING

3. **Model Training & Evaluation**
   - Evaluated using:
     - **Accuracy**
     - **Precision**
     - **Recall** (Key Metric)
     - **F1-Score**
     - **ROC-AUC**
   - Plotted confusion matrix and ROC curves for visual insight

---

## 📈 Results

| Model            | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | ~99.2% | High      | Moderate | Good    | Good    |
| Random Forest       | ~99.9% | High      | High     | High    | Excellent |
| XGBoost             | ~99.9% | Very High | High     | High    | Excellent |

> ✅ **Random Forest and XGBoost** offered the best trade-off between fraud detection and false positives.

---

## 🛠 Tech Stack

- Python
- Jupyter Notebook
- Scikit-learn
- XGBoost / LightGBM
- Matplotlib / Seaborn
- Pandas / NumPy

---

## 🚀 Future Enhancements

- Build an API for real-time fraud detection (Flask/FastAPI)
- Deploy using Streamlit for UI
- Use raw transaction data for deeper feature engineering
- Experiment with deep learning (Autoencoders, LSTM)

---

## 📌 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/CreditCardFraudDetection.git
   cd CreditCardFraudDetection
