# Titanic Survival Prediction

## Problem

The goal of this project is to predict whether a passenger survived the Titanic disaster based on features such as age, sex, ticket class, fare, and embarkation point.

This is a binary classification problem where:
- 1 = Survived
- 0 = Did not survive

---

## Dataset

- Source: Seaborn Titanic dataset
- Target variable: survived

Selected features:
- pclass (ticket class)
- sex
- age
- fare
- embarked

---

## Workflow

1. Data loading and exploration  
2. Handling missing values  
3. Feature selection  
4. Train-test split  
5. Data preprocessing (scaling and encoding)  
6. Model training  
7. Model evaluation  
8. Model comparison  

---

## Data Preprocessing

- Missing values:
  - Age filled with median
  - Embarked filled with mode

- Numerical features:
  - Scaled using StandardScaler

- Categorical features:
  - Encoded using OneHotEncoder

- Preprocessing handled using ColumnTransformer and Pipeline

---

## Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## Key Concepts Learned

- Difference between classification and regression
- Understanding confusion matrix
- Trade-off between precision and recall
- Why accuracy alone can be misleading
- How to use pipelines for clean preprocessing and modeling

---

## Results Summary

| Model | Accuracy | Precision | Recall | F1 |
|------|----------|----------|--------|----|
| Logistic Regression | ... | ... | ... | ... |
| Decision Tree | ... | ... | ... | ... |
| Random Forest | ... | ... | ... | ... |

---

## Key Insights

- Sex and passenger class are strong predictors of survival
- Tree-based models can capture non-linear relationships better
- Logistic Regression provides a good baseline model
- Model selection should consider recall and precision, not just accuracy

---

## Files

- notebook.ipynb: Full implementation of the project
- README.md: Project documentation

---

## How to Run

1. Install dependencies:
   pip install -r requirements.txt

2. Launch Jupyter Notebook:
   jupyter notebook

3. Open notebook.ipynb and run all cells

---

## Future Improvements (for ver 2)

- Hyperparameter tuning (GridSearchCV)
- Feature engineering (e.g., family size, title extraction)
- Handling class imbalance
- Trying additional models (SVM, Gradient Boosting)

---

## Conclusion

This project demonstrates a complete classification workflow, including preprocessing, model training, and evaluation. It highlights the importance of choosing the right evaluation metrics and understanding model performance beyond accuracy.

## Model Comparison Conclusion

The Logistic Regression model achieved an accuracy of 0.79, suggesting good overall classification performance.

With a precision of 0.76 and recall of 0.72, the model demonstrates a balanced ability to correctly identify survivors while limiting false positives. The F1 score of 0.74 further confirms this balance between precision and recall.

Overall, the model performs consistently across all metrics and serves as a strong baseline for this classification task.