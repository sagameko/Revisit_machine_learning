# Loan Approval Prediction

## Overview

This project focuses on building a machine learning model to predict whether a loan application should be approved based on a set of financial and demographic features.

The goal is to simulate a simplified version of a real-world loan approval system, where decisions are influenced by factors such as credit score, income, loan size, and asset values.

---

## Problem Statement

Given applicant information, the model predicts:

- 1 = Loan Approved  
- 0 = Loan Rejected  

This is a binary classification problem with direct relevance to financial decision-making.

---

## Dataset

The dataset contains the following key features:

- no_of_dependents  
- education  
- self_employed  
- income_annum  
- loan_amount  
- loan_term  
- cibil_score  
- residential_assets_value  
- commercial_assets_value  
- luxury_assets_value  
- bank_asset_value  
- loan_status (target)

The data includes both numerical and categorical variables, making it a good representation of real-world structured data.

---

## Approach

The project follows a standard machine learning workflow:

1. Data loading and initial exploration  
2. Data cleaning and target encoding  
3. Feature separation (numerical and categorical)  
4. Train-test split  
5. Preprocessing using ColumnTransformer  
   - StandardScaler for numerical features  
   - OneHotEncoder for categorical features  
6. Model training using Pipeline  
7. Model evaluation using multiple metrics  
8. Model comparison  

---

## Models Used

- Logistic Regression  
- Random Forest Classifier  

Logistic Regression is used as a baseline model, while Random Forest is used to capture more complex, non-linear relationships.

---

## Evaluation Metrics

Model performance is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

These metrics help assess not only overall performance but also the trade-off between correctly approving loans and avoiding risky approvals.

---

## Key Insights

- Credit score (cibil_score) is expected to be one of the most important factors in loan approval decisions  
- Income and asset values provide strong signals of repayment capability  
- Loan amount introduces financial risk and affects approval likelihood  
- Tree-based models such as Random Forest can better capture complex relationships compared to linear models  

---

## Business Considerations

In a loan approval system:

- False Positive: Approving a risky applicant → potential financial loss  
- False Negative: Rejecting a reliable applicant → lost business opportunity  

Choosing the right balance between precision and recall depends on the organization's risk tolerance.

---

## Results Summary

| Model | Accuracy | Precision | Recall | F1 |
|------|----------|----------|--------|----|
| Logistic Regression | ... | ... | ... | ... |
| Random Forest | ... | ... | ... | ... |

---

## Files

- notebook.ipynb: Full implementation of the project  
- loan_data.csv: Dataset used for training and evaluation  
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

- The model is trained on a single dataset and may not generalize to all real-world scenarios  
- No hyperparameter tuning has been applied yet  
- Feature engineering is minimal in this version  

---

## Future Improvements (Version 2)

This project represents the first version of the solution. I plan to revisit and improve it in a future iteration.

Planned improvements include:

- Hyperparameter tuning using GridSearchCV  
- Threshold tuning using predicted probabilities  
- Feature engineering (e.g., financial ratios)  
- Model interpretability (feature importance analysis)  
- Better handling of class imbalance if present  

---

## Conclusion

This project demonstrates a complete classification workflow using a realistic financial dataset. It highlights the importance of proper preprocessing, model evaluation, and understanding business trade-offs in machine learning applications.

This is part of a broader effort to rebuild and strengthen my machine learning and Python fundamentals through structured, hands-on projects.