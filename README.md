# 💳 Credit Card Fraud Detection using Machine Learning

<p align="center">

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white">
  <img src="https://img.shields.io/badge/Kaggle-Dataset-20BEFF?logo=kaggle&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas">
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn">
  <img src="https://img.shields.io/badge/Imbalanced--Learn-SMOTE-009688">
  <img src="https://img.shields.io/badge/XGBoost-Gradient%20Boosting-EC6B23">
  <img src="https://img.shields.io/badge/SHAP-Explainable%20AI-FF6F00">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C">
  <img src="https://img.shields.io/badge/Seaborn-EDA-4C72B0">
</p>

---

# 📑 Table of Contents

- 📌 Overview
- 🎯 Objectives
- 📂 Dataset
- 🏗️ Project Architecture
- ⚙️ Technologies Used
- 📊 Exploratory Data Analysis (EDA)
- 🤖 Model Building
- 📈 Results
- 📉 Performance Metrics
- 🔍 Explainable AI (SHAP)
- 📈 Output Visualizations
- 📊 Performance Summary
- 🎯 Business Impact
- 💼 Real-World Applications
- 📊 Model Performance Summary
- 🏗 System Architecture
- 📌 Future Improvements
- 🧠 Key Learnings

---

# 📌 Overview

Credit card fraud has become one of the fastest-growing financial crimes worldwide, resulting in billions of dollars in losses every year. As digital payment systems continue to expand, detecting fraudulent transactions in real time has become a critical challenge for financial institutions. Traditional rule-based fraud detection systems often struggle to identify new fraud patterns and generate a large number of false alarms.

This project develops an intelligent **Credit Card Fraud Detection System** using the **Random Forest Machine Learning algorithm** to accurately classify transactions as **Fraudulent** or **Genuine**. The project includes data preprocessing, exploratory data analysis (EDA), model training, performance evaluation, and Explainable AI using SHAP to provide transparency in predictions. The solution demonstrates how machine learning can significantly improve fraud detection while minimizing financial risks.

---

# 🎯 Objectives

The primary objectives of this project are:

- 🎯 Detect fraudulent credit card transactions with high accuracy.
- 📊 Perform exploratory data analysis to understand transaction patterns.
- 🧹 Clean and preprocess the dataset for effective model training.
- 🤖 Train a Random Forest classification model.
- 📉 Evaluate model performance using multiple evaluation metrics.
- 🔍 Interpret model predictions using SHAP Explainable AI.
- 💼 Generate meaningful business insights from the analysis.

---

# 📂 Dataset

The project uses the **Credit Card Fraud Detection Dataset**, which contains anonymized transaction records collected from European cardholders.

| 📌 Attribute | 📊 Value |
|-------------|----------|
| Dataset Size | 284,808 Transactions |
| Features | 31 Columns |
| Genuine Transactions | 284,315 |
| Fraud Transactions | 493 |
| Fraud Percentage | 0.17% |
| Target Variable | Class |

### 📋 Features Included

- ⏰ Time
- 💰 Amount
- 🔢 V1 to V28 (PCA-transformed features)
- 🎯 Class (Target Variable)

**Target Labels**

- ✅ 0 → Genuine Transaction
- 🚨 1 → Fraudulent Transaction

---

# 🏗️ Project Architecture

The project follows a structured machine learning workflow to build an accurate fraud detection model.

```text
Credit Card Dataset
        │
        ▼
Data Preprocessing
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Train-Test Split
        │
        ▼
Random Forest Model
        │
        ▼
Prediction
        │
        ▼
Model Evaluation
        │
        ▼
Feature Importance
        │
        ▼
SHAP Explainability
        │
        ▼
Business Insights
```

---

# ⚙️ Technologies Used

| 🛠 Technology | 📌 Purpose |
|--------------|------------|
| 🐍 Python | Programming Language |
| 🐼 Pandas | Data Manipulation |
| 🔢 NumPy | Numerical Computation |
| 📊 Matplotlib | Data Visualization |
| 🤖 Scikit-Learn | Machine Learning |
| 🧠 SHAP | Explainable AI |
| 💾 Joblib | Model Saving |
| ☁️ Google Colab | Development Environment |

---

# 📊 Exploratory Data Analysis (EDA)

EDA was performed to understand the characteristics of the dataset before model development.

### 📌 Analysis Performed

- 📊 Fraud vs Genuine Transaction Distribution
- 🔥 Correlation Heatmap
- 💰 Transaction Amount Distribution
- ⏰ Transaction Time Distribution

### 🔍 Key Observations

- Fraud cases represent only **0.17%** of the dataset.
- The dataset is highly imbalanced.
- Most PCA features show very low correlation.
- Transaction amounts are positively skewed.
- Transaction activity varies over time.

These findings helped in selecting appropriate evaluation metrics and building a robust machine learning model.

---

# 🤖 Model Building

A **Random Forest Classifier** was selected for fraud detection because of its excellent performance on tabular datasets and its ability to handle nonlinear relationships.

### Model Development Steps

- 📥 Load Dataset
- 🧹 Data Cleaning
- ✂️ Train-Test Split
- 🌳 Train Random Forest Model
- 🎯 Predict Transaction Class
- 📈 Evaluate Performance
- ⭐ Feature Importance Analysis
- 🧠 SHAP Explainability
- 💾 Save Trained Model

---

# 📈 Results

The developed model achieved excellent performance in identifying fraudulent transactions.

### 📌 Highlights

- ✅ Successfully detected **94 out of 95** fraud transactions.
- ✅ Missed only **one** fraudulent transaction.
- ✅ Achieved an outstanding **ROC-AUC score of 1.00**.
- ✅ Generated very few false alarms.
- ✅ Performed effectively despite severe class imbalance.

---

# 📉 Performance Metrics

Multiple evaluation metrics were used to assess the model's effectiveness.

| 📊 Metric | 📈 Value |
|-----------|----------|
| Accuracy | **99.82%** |
| Precision | **0.48** |
| Recall | **0.99** |
| F1-Score | **0.65** |
| ROC-AUC | **1.00** |
| Average Precision | **0.95** |

### 📌 Why These Metrics?

- 🎯 Accuracy measures overall prediction correctness.
- 📉 Precision evaluates how many predicted frauds are actually fraud.
- 📈 Recall measures the model's ability to detect fraudulent transactions.
- ⚖️ F1-Score balances precision and recall.
- 📊 ROC-AUC evaluates discrimination capability.
- 📈 Average Precision is ideal for highly imbalanced datasets.

---

# 🔍 Explainable AI (SHAP)

To improve model transparency, **SHAP (SHapley Additive exPlanations)** was used.

### Benefits of SHAP

- 🧠 Explains individual predictions.
- 🔍 Identifies feature contributions.
- 📊 Improves model interpretability.
- 🤝 Builds trust among stakeholders.
- 📋 Supports regulatory compliance.

---

# 📈 Output Visualizations

The project generates several visualizations to analyze both the dataset and model performance.

| 📊 Visualization | 📝 Purpose |
|------------------|------------|
| 📊 Fraud vs Genuine Transactions | Shows class imbalance |
| 🔥 Correlation Heatmap | Displays feature relationships |
| 💰 Transaction Amount Distribution | Analyzes transaction values |
| ⏰ Transaction Time Distribution | Studies transaction timing |
| 📉 Confusion Matrix | Evaluates prediction results |
| 📈 ROC Curve | Measures classification capability |
| 📊 Precision-Recall Curve | Evaluates minority class performance |
| ⭐ Feature Importance | Identifies influential variables |
| 🧠 SHAP Summary Plot | Explains model predictions |

---

# 📊 Performance Summary

The Random Forest classifier demonstrated excellent fraud detection capability.

| 📌 Metric | 📈 Value |
|-----------|----------|
| Dataset Size | 284,808 |
| Fraud Cases | 493 |
| Accuracy | **99.82%** |
| ROC-AUC | **1.00** |
| Average Precision | **0.95** |
| Fraud Detected | **94 / 95** |
| False Negatives | **1** |
| False Positives | **101** |

### Summary

- ✔ High fraud detection accuracy.
- ✔ Extremely low false negative rate.
- ✔ Excellent discrimination between fraud and genuine transactions.

---

# 🎯 Business Impact

The developed solution provides significant value to financial institutions.

### 💼 Benefits

- 💳 Reduces fraudulent financial losses.
- 🚨 Detects fraud in near real-time.
- 📉 Minimizes false transaction blocks.
- 🤖 Reduces manual investigation effort.
- 🔒 Improves payment security.
- 📊 Supports data-driven fraud management.

---

# 💼 Real-World Applications

The project can be applied across multiple industries.

- 🏦 Banking
- 💳 Credit Card Companies
- 📱 Digital Payment Platforms
- 🛒 E-Commerce
- 💰 FinTech
- 🛡 Cybersecurity
- 📈 Financial Risk Analytics
- 🌐 Online Payment Gateways
- 💵 Digital Wallet Services

---

# 📊 Model Performance Summary

| 📊 Evaluation Metric | 📈 Result | 📌 Interpretation |
|----------------------|-----------|-------------------|
| Accuracy | **99.82%** | Excellent overall prediction accuracy |
| Precision | **0.48** | Moderate precision due to class imbalance |
| Recall | **0.99** | Nearly all fraud transactions detected |
| F1-Score | **0.65** | Good balance of precision and recall |
| ROC-AUC | **1.00** | Outstanding classification performance |
| Average Precision | **0.95** | Excellent minority class prediction |

### Key Findings

- ✔ Excellent fraud detection capability.
- ✔ Strong model generalization.
- ✔ Very low false negative rate.
- ✔ Suitable for real-world fraud detection systems.

---

# 🏗 System Architecture

```text
                  Credit Card Dataset
                           │
                           ▼
                Data Preprocessing
                           │
                           ▼
             Exploratory Data Analysis
                           │
                           ▼
            Random Forest Model Training
                           │
                           ▼
                 Fraud Prediction Model
                           │
            ┌──────────────┴──────────────┐
            ▼                             ▼
    Performance Evaluation       Feature Importance
            │                             │
            └──────────────┬──────────────┘
                           ▼
                SHAP Explainability
                           │
                           ▼
             Fraud / Genuine Prediction
                           │
                           ▼
                Business Decision Support
```

---

# 📌 Future Improvements

The project can be further enhanced by integrating advanced machine learning techniques and deployment strategies.

- 🚀 XGBoost Classifier
- ⚡ LightGBM
- 🧠 CatBoost
- 🤖 Deep Neural Networks
- 📊 Autoencoder-based Anomaly Detection
- 🌐 Streamlit Web Application
- ☁️ Cloud Deployment (AWS, Azure, GCP)
- 🐳 Docker Containerization
- ⚙️ GitHub Actions for CI/CD
- 📡 REST API using FastAPI
- 📲 Real-Time Fraud Alert System

---

# 🧠 Key Learnings

Throughout this project, several important concepts in machine learning, data analysis, and fraud detection were explored.

### 📚 Technical Learnings

- 🐍 Data preprocessing using Pandas.
- 📊 Exploratory Data Analysis for understanding datasets.
- 🤖 Building classification models using Random Forest.
- 📉 Evaluating imbalanced datasets using appropriate metrics.
- 🔍 Interpreting model predictions with SHAP.
- 💾 Saving and reusing trained machine learning models.

### 💼 Business Learnings

- Fraud detection requires prioritizing recall over accuracy.
- Explainable AI increases confidence in machine learning systems.
- Data-driven fraud detection significantly reduces financial risks.
- Machine learning can automate fraud monitoring and improve operational efficiency.

---

# 👨‍💻 Author

## **Anns Jana**

**Data Science & Machine Learning Enthusiast**

📌 Passionate about solving real-world business problems using Data Science, Machine Learning, Artificial Intelligence, and Business Intelligence.
