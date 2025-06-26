# 🧠 KNIME Workflow Notes – Monkeypox Classification Project

This document outlines the machine learning workflow built in **KNIME Analytics Platform** to classify Monkeypox cases using clinical data from patients.

---

## 🧩 Workflow Overview

The complete KNIME workflow consists of the following key components:

### 1. **Data Input**
- **CSV Reader** node: Imports the Monkeypox dataset.
- Output: 25,000 patient records with 12 attributes (11 features, 1 target).

### 2. **Data Exploration**
- **Table View**: Quick inspection of null values, value distributions.
- **Missing Value** node: (if needed) handles incomplete records.

### 3. **Data Preprocessing**
- **Column Filter**: Selects only relevant attributes for modeling.
- **Partitioning**: Splits data into training (70%) and test (30%) sets.

---

## ⚙️ Model Training

Each algorithm was trained using its respective learner node:

### 🔹 Naive Bayes
- **Naive Bayes Learner**
- **Naive Bayes Predictor**

### 🔹 Logistic Regression
- **Logistic Regression Learner**
- **Logistic Regression Predictor**

### 🔹 Random Forest
- **Random Forest Learner**
- **Random Forest Predictor**

---

## 📊 Model Evaluation

Each model was evaluated using:

- **Scorer** node → Generates confusion matrix.
- **ROC Curve** node → Evaluates model via AUC.
- **Numeric Scorer** or **Column Aggregator** → Checks accuracy, precision, recall.

---

## 📈 Results Summary

| Algorithm           | Accuracy | AUC     |
|---------------------|----------|---------|
| Naive Bayes         | 69.73%   | ~0.89   |
| Logistic Regression | 66.60%   | ~0.87   |
| Random Forest       | 66.43%   | **0.891**

- Naive Bayes had the highest accuracy.
- Random Forest achieved the best AUC performance.

---

## 📌 Screenshot of Workflow (Add your image here)

> ![KNIME Workflow Screenshot](../results/knime_workflow_screenshot.png)

---

## 💬 Notes
- KNIME makes it easy to experiment with various algorithms without writing code.
- Future improvement: test additional features, apply cross-validation, and try advanced models like XGBoost.

---

*Created by Hanif Fachrizal & Team – Universitas Bina Sarana Informatika | 2024*
