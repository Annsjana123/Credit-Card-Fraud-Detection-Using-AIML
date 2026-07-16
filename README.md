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

# 📖 Table of Contents

- 📌 Overview
- 🎯 Objectives
- 📂 Dataset
- 🏗️ Project Architecture
- ⚙️ Technologies
- 📊 Exploratory Data Analysis
- 🤖 Model Building
- 📈 Results
- 📉 Performance Metrics
- 🔍 Explainable AI
- 📌 Future Improvements
- 🧠 Key Learnings
- 📚 Technical Learnings
- 💼 Practical Learnings

---
# 💳 Credit Card Fraud Detection using Machine Learning

An end-to-end Machine Learning project that detects fraudulent credit card transactions using data preprocessing, exploratory data analysis, feature engineering, class imbalance handling, and multiple classification algorithms. The project focuses on maximizing fraud detection while minimizing false positives through robust model evaluation and explainable AI techniques.

---

# 🎯 Objectives

The primary objectives of this project are:

- 💳 Detect fraudulent credit card transactions with high accuracy.
- ⚡ Identify suspicious transactions in real-time.
- 📉 Minimize financial losses caused by fraudulent activities.
- ⚖️ Handle highly imbalanced datasets effectively.
- 🤖 Compare multiple Machine Learning algorithms.
- 📊 Evaluate models using fraud-specific performance metrics.
- 🔍 Improve transparency using Explainable AI (SHAP/LIME).
- 🚀 Build a scalable fraud detection pipeline for future deployment.

---

# 📂 Dataset

### Dataset Information

| Attribute | Details |
|-----------|----------|
| Dataset | Credit Card Fraud Detection Dataset |
| Source | Kaggle / European Cardholders Dataset |
| Records | 284,807 Transactions |
| Features | 31 Columns |
| Fraud Cases | 492 |
| Legitimate Cases | 284,315 |
| Fraud Percentage | 0.172% |
| Target Variable | Class |
| Dataset Type | Highly Imbalanced Binary Classification |

### Feature Description

The dataset contains:

- **Time** → Seconds elapsed between transactions
- **V1 – V28** → PCA-transformed confidential features
- **Amount** → Transaction amount
- **Class**
  - 0 → Legitimate Transaction
  - 1 → Fraudulent Transaction

### Dataset Challenges

- ⚠️ Extreme class imbalance
- 🔒 Anonymous features due to privacy
- 💰 Fraud transactions are extremely rare
- 📈 Requires specialized evaluation metrics

---

# 🏗️ Project Architecture

```text
                 Credit Card Dataset
                        │
                        ▼
              Data Loading & Inspection
                        │
                        ▼
                Data Cleaning
                        │
                        ▼
          Exploratory Data Analysis (EDA)
                        │
                        ▼
          Feature Scaling (Amount, Time)
                        │
                        ▼
      Handling Class Imbalance (SMOTE)
                        │
                        ▼
          Train-Test Split (80:20)
                        │
                        ▼
        Machine Learning Model Training
                        │
                        ▼
     Random Forest / XGBoost / LightGBM
                        │
                        ▼
             Model Evaluation
                        │
                        ▼
        Explainable AI (SHAP & LIME)
                        │
                        ▼
          Fraud Prediction Pipeline
```

---

# ⚙️ Technologies

## 🖥️ Programming Language

- Python 3.x

## 📚 Libraries

### Data Processing

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn
- Plotly

### Machine Learning

- Scikit-learn
- XGBoost
- LightGBM
- Imbalanced-learn (SMOTE)

### Explainable AI

- SHAP
- LIME

### Notebook

- Google Colab
- Jupyter Notebook

### Version Control

- Git
- GitHub

---

# 📊 Exploratory Data Analysis

EDA helps understand the characteristics of the dataset before model development.

### ✔️ Performed Analysis

- 📌 Dataset overview
- 📌 Missing value analysis
- 📌 Duplicate record detection
- 📌 Class distribution
- 📌 Transaction amount analysis
- 📌 Time distribution
- 📌 Feature correlation heatmap
- 📌 Fraud vs Legit comparison
- 📌 Outlier detection
- 📌 PCA feature visualization

### 📈 Visualizations

- 📊 Class Distribution Count Plot
- 📈 Transaction Amount Histogram
- 📉 Transaction Time Distribution
- 🔥 Correlation Heatmap
- 📦 Boxplots
- 📍 Scatter Plots
- 📊 KDE Plots
- 🥧 Fraud Percentage Pie Chart

### Key Insights

- Only **0.172%** of transactions are fraudulent.
- Most transactions are legitimate.
- Fraudulent transactions often involve smaller transaction amounts.
- Severe class imbalance makes accuracy alone misleading.
- Feature engineering and sampling techniques significantly improve model performance.

---

# 🤖 Model Building

Several machine learning algorithms were trained and compared.

### Data Preprocessing

- ✅ Missing value verification
- ✅ Duplicate removal
- ✅ StandardScaler for Amount and Time
- ✅ Train-Test Split
- ✅ SMOTE Oversampling
- ✅ Feature Selection

### Models Implemented

| Model | Purpose |
|--------|----------|
| Logistic Regression | Baseline Model |
| Decision Tree | Rule-based Classification |
| Random Forest | Ensemble Learning |
| XGBoost | Gradient Boosting |
| LightGBM | Fast Boosting Algorithm |
| Support Vector Machine | Hyperplane Classification |
| K-Nearest Neighbors | Distance-based Learning |

### Best Performing Model

🏆 **Random Forest / XGBoost** achieved the best balance between fraud detection and minimizing false alarms.

---

# 📈 Results

The trained models successfully identified fraudulent transactions with high precision and recall.

### Achievements

- ✅ Excellent fraud detection capability
- ✅ High ROC-AUC Score
- ✅ Low False Positive Rate
- ✅ Better generalization after SMOTE
- ✅ Reliable prediction pipeline

### Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|--------|----------|-----------|---------|----------|----------|
| Logistic Regression | High | Good | Moderate | Good | High |
| Decision Tree | High | Good | Good | Good | High |
| Random Forest | Excellent | Excellent | Excellent | Excellent | Excellent |
| XGBoost | Excellent | Excellent | Excellent | Excellent | Excellent |
| LightGBM | Excellent | Excellent | Excellent | Excellent | Excellent |

---

# 📉 Performance Metrics

Since fraud detection involves highly imbalanced data, multiple evaluation metrics are considered.

### Metrics Used

- 🎯 Accuracy
- 🎯 Precision
- 🎯 Recall
- 🎯 F1 Score
- 🎯 ROC-AUC Score
- 🎯 PR-AUC Score
- 🎯 Confusion Matrix

### Why Accuracy Isn't Enough?

Because over **99%** of transactions are legitimate, a model predicting every transaction as legitimate would still achieve very high accuracy while failing to detect fraud.

Therefore, **Precision**, **Recall**, **F1 Score**, and **ROC-AUC** provide a much better assessment of model performance.

---

# 🔍 Explainable AI

To improve transparency and interpretability, Explainable AI techniques were used.

### SHAP (SHapley Additive Explanations)

✔ Explains feature contribution for every prediction.

Benefits:

- Feature importance ranking
- Global model interpretation
- Local prediction explanation

### LIME (Local Interpretable Model-Agnostic Explanations)

Provides explanations for individual predictions.

Benefits:

- Understands why a transaction was classified as fraud
- Builds trust in model predictions
- Supports auditing and compliance

### Explainability Outputs

- 📊 SHAP Summary Plot
- 📈 SHAP Feature Importance
- 📍 SHAP Force Plot
- 🔍 LIME Prediction Explanation

---

# 📌 Future Improvements

Future enhancements planned for this project include:

- 🚀 Deep Learning models (ANN, CNN)
- ⚡ Real-time fraud detection API
- 🌐 Streamlit web application
- ☁️ Cloud deployment (AWS, Azure, GCP)
- 🔄 Continuous model retraining
- 📱 Mobile-friendly prediction interface
- 📊 Interactive Power BI Dashboard
- 🧠 AutoML model optimization
- 📈 Real-time transaction monitoring
- 🔔 Instant fraud alert notification system
- 🗄️ Integration with SQL databases
- 🧩 MLOps pipeline using Docker and Kubernetes

---

## 🌟 Project Highlights

- 💳 Real-world financial fraud detection use case
- 📊 Comprehensive Exploratory Data Analysis
- ⚖️ Handles highly imbalanced data using SMOTE
- 🤖 Multiple Machine Learning models
- 📈 Robust evaluation with fraud-specific metrics
- 🔍 Explainable AI using SHAP and LIME
- 🚀 Deployment-ready prediction pipeline
- 📚 Well-structured and reproducible workflow

---

# 🧠 Key Learnings

Throughout this project, several important concepts in Data Science and Machine Learning were explored and applied to solve a real-world fraud detection problem.

### 📚 Technical Learnings

- 💳 Understood the challenges of detecting fraudulent financial transactions.
- 📊 Performed comprehensive Exploratory Data Analysis (EDA) to identify hidden patterns and trends.
- 🧹 Learned effective data preprocessing techniques, including handling duplicates, scaling numerical features, and preparing data for model training.
- ⚖️ Gained practical experience in handling highly imbalanced datasets using **SMOTE (Synthetic Minority Over-sampling Technique)**.
- 🤖 Built and compared multiple Machine Learning classification models such as Logistic Regression, Decision Tree, Random Forest, XGBoost, and LightGBM.
- 📈 Evaluated models using fraud-specific performance metrics including Precision, Recall, F1 Score, ROC-AUC, and Confusion Matrix instead of relying solely on accuracy.
- 🔍 Applied Explainable AI techniques using **SHAP** and **LIME** to interpret model predictions and improve transparency.
- 🚀 Developed a complete end-to-end Machine Learning pipeline suitable for real-world fraud detection applications.

### 💼 Practical Learnings

- ✔ Importance of data quality before model training.
- ✔ Why class imbalance significantly impacts prediction performance.
- ✔ How ensemble learning models outperform traditional algorithms for fraud detection.
- ✔ The role of explainability in building trustworthy AI systems.
- ✔ Best practices for developing reproducible and scalable Data Science projects.

---

# 👨‍💻 Author

## **Anns Jana**

**Data Science & Machine Learning Enthusiast**

📌 Passionate about solving real-world business problems using Data Science, Machine Learning, Artificial Intelligence, and Business Intelligence.
