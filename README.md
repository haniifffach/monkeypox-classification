# Monkeypox Classification using Machine Learning

This project compares three classification algorithms—Naive Bayes, Logistic Regression, and Random Forest—for predicting Monkeypox infection from clinical symptom data.

## 📊 Dataset
- 25,000 patient records
- 11 input features (e.g., Rectal Pain, HIV Infection, Oral Lesions)
- 1 target output: Monkeypox (Yes/No)

> ⚠️ Dataset is not publicly available due to privacy constraints. Only sample structure is provided.

## 🧰 Tools Used
- KNIME Analytics Platform
- Confusion Matrix and ROC for evaluation

## 📈 Evaluation Results

| Algorithm           | Accuracy | AUC     |
|---------------------|----------|---------|
| Naive Bayes         | 69.73%   | -       |
| Logistic Regression | 66.60%   | -       |
| Random Forest       | 66.43%   | 0.891   |

## 📂 Project Structure
- `data/` : Sample dataset
- `notebooks/` : Workflow notes
- `results/` : Evaluation output
- `report/` : Final project report (PDF)
