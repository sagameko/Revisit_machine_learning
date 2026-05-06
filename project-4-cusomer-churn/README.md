# Customer Churn Prediction

## Overview

This project focuses on predicting whether a customer is likely to leave a company based on their demographic and service usage data.

Customer churn prediction is a common real-world problem, especially in industries such as telecommunications, banking, and subscription-based services. The goal is to identify customers at risk of leaving so that the business can take proactive actions to retain them.

---

## Problem Statement

The task is to build a binary classification model:

- 1 = Customer will churn  
- 0 = Customer will stay  

The model uses customer-related features to estimate the likelihood of churn.

---

## Dataset

The dataset includes a mix of numerical and categorical features such as:

- Customer demographics (e.g., gender, senior status)
- Account information (e.g., tenure, contract type)
- Services used (e.g., internet service, phone service)
- Billing details (e.g., monthly charges, total charges)

Target variable:

- Churn (Yes / No)

---

## Approach

The project follows a structured machine learning workflow:

1. Data loading and exploration  
2. Data cleaning (handling missing values and type conversion)  
3. Feature selection  
4. Train-test split with stratification  
5. Preprocessing using ColumnTransformer  
   - StandardScaler for numerical features  
   - OneHotEncoder for categorical features  
6. Model training using Pipeline  
7. Model evaluation using multiple metrics  
8. Model comparison  

---

## Models Used

- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  

Logistic Regression provides a strong and interpretable baseline, while tree-based models capture more complex patterns in the data.

---

## Evaluation Metrics

Model performance is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

These metrics provide a more complete understanding of model performance, especially in classification problems where class imbalance may exist.

---

## Key Insights

- Customer tenure and contract type are strong indicators of churn  
- Customers with month-to-month contracts are more likely to churn  
- Higher monthly charges may correlate with higher churn risk  
- Tree-based models can capture non-linear relationships, but Logistic Regression often provides a stable and interpretable baseline  

---

## Business Considerations

In a churn prediction system:

- False Negative: The model predicts a customer will stay, but they actually churn  
  This is costly because the business loses the customer without taking preventive action  

- False Positive: The model predicts a customer will churn, but they actually stay  
  This may lead to unnecessary retention efforts, but is usually less costly  

Because of this, recall is often more important than accuracy in churn prediction.

---

## Results Summary

| Model | Accuracy | Precision | Recall | F1 |
|------|----------|----------|--------|----|
| Logistic Regression | ... | ... | ... | ... |
| Decision Tree | ... | ... | ... | ... |
| Random Forest | ... | ... | ... | ... |

---

## Files

- notebook.ipynb: Full implementation  
- churn_data.csv: Dataset used  
- README.md: Project documentation  

---

## How to Run

1. Install dependencies:
   pip install -r requirements.txt

2. Start Jupyter Notebook:
   jupyter notebook

3. Open notebook.ipynb and run all cells

---

## Limitations

- No hyperparameter tuning has been applied yet  
- Limited feature engineering  
- Model performance may vary depending on dataset quality  

---

## Future Improvements (Version 2)

This is the first version of the project. I plan to revisit and improve it in a future iteration.

Planned improvements include:

- Hyperparameter tuning using GridSearchCV  
- Threshold tuning using predicted probabilities  
- Feature engineering (e.g., customer lifetime value, tenure grouping)  
- Handling class imbalance more explicitly  
- Model explainability (feature importance, SHAP values)  

---

## Conclusion

This project demonstrates a complete classification workflow applied to a real-world business problem. It highlights the importance of proper preprocessing, model evaluation, and understanding the trade-offs between different performance metrics.

This work is part of a structured effort to rebuild and strengthen my machine learning and Python skills through practical, end-to-end projects.