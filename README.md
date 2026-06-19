# Bank-Loan-Default-Prediction
# Financial Return Categorization using Machine Learning
This repository contains an end-to-end data science and machine learning pipeline designed to predict and classify financial return categories (`retcat`). The project implements, benches, and compares multiple predictive models to identify the most accurate framework for performance classification.

## 📌 Project Overview
The objective of this project is to analyze historical financial metrics to classify returns into distinct risk or performance categories. By automating this process, the pipeline serves as a scalable tool for corporate finance analysis, investment tracking, and data-driven decision-making.

The project fulfills a structured financial data analysis workflow:
1. **Data Cleaning & Management:** Resolving structural missing data points.
2. **Feature Engineering:** Label encoding categorical targets and standardizing feature spaces.
3. **Multi-Model Benchmarking:** Training and evaluating 6 distinct machine learning algorithms.

---

## 📊 Dataset & Preprocessing
* **Primary Dataset:** `USA-RV (Dataset).xlsx`
* **Target Variable:** `retcat` (Categorical return classification)
* **Missing Value Management:** Handled uniformly using median imputation to preserve data distribution stability.
* **Feature Scaling:** Applied `StandardScaler` to normalize numerical variables, ensuring distance-based and gradient-based algorithms perform optimally.

---

## 🤖 Implemented Models
To find the optimal predictive architecture, the dataset was evaluated across a diverse suite of classical machine learning algorithms using a **70% training and 30% testing split**:

* **Logistic Regression** (Optimized with extended iterations)
* **Decision Tree Classifier**
* **Random Forest Classifier** (Ensemble-based learning)
* **Support Vector Machine (SVM)**
* **Gaussian Naive Bayes**
* **K-Nearest Neighbors (KNN)**

---

## 📈 Evaluation Matrix
Models are rigorously tested to ensure generalizability and prevent overfitting using:
* **Stratified K-Fold Cross-Validation** (Ensuring class balance across training folds)
* **Accuracy Scores**
* **Precision, Recall, and F1-Scores** 
* **Confusion Matrices**

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning Framework:** `scikit-learn`
* **File Processing:** `openpyxl` (for Excel dataset ingestion)
* **Deep Learning Architecture:** `tensorflow` / `keras` (Environment configured)

---

## 🚀 How to Run

### 1. Prerequisites
Install the required dependencies using pip:
```bash
pip install pandas numpy scikit-learn openpyxl tensorflow
python Loan_Deafault.py
