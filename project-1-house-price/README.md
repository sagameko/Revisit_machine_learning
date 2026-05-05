# House Price Prediction

## Problem

The goal of this project is to predict house prices based on various features such as income, population, and housing characteristics.

---

## Dataset

- Source: California Housing Dataset (Scikit-learn)
- Target: Median House Value

---

## Workflow

1. Data loading and exploration
2. Data visualization (EDA)
3. Feature preparation
4. Train-test split
5. Data scaling
6. Model training
7. Model evaluation
8. Model comparison

---

## Models Used

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor

---

## Evaluation Metrics

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

---

## Key Insights

- Random Forest performed the best due to its ability to capture non-linear relationships
- Median income (MedInc) is the most important feature affecting house prices
- Linear models struggled due to the non-linear nature of the data

---

## Results Summary

| Model | MAE | RMSE | R² |
|------|-----|------|----|
| Linear Regression | ... | ... | ... |
| Ridge | ... | ... | ... |
| Lasso | ... | ... | ... |
| Random Forest | ... | ... | ... |

---

## 📁 Files

- `notebook.ipynb` → Full implementation
- `requirements.txt` → Dependencies

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook