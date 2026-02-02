# Feature Engineering and Tree-Based Models for Income Prediction

## Project Overview
This project applies Decision Tree, Random Forest, XGBoost, and LightGBM models on the **Adult Census Income** dataset to predict whether a person earns **more than 50K** per year.  
The focus is on understanding tree-based algorithms, ensemble methods, hyperparameter tuning, and model interpretability.

---

## Dataset
- Source: Kaggle / OpenML Adult Census dataset  
- Target Variable: `income (>50K or <=50K)`  
- Features: age, education, occupation, hours-per-week, capital gain, marital status, etc.

---

## Steps Performed

### 1. Decision Tree
- Implemented Decision Tree classifier  
- Explained:
  - Gini Impurity vs Entropy  
  - Overfitting  
  - Role of max_depth, min_samples_split, min_samples_leaf, max_features  
- Evaluated using Accuracy, Precision, Recall

### 2. Random Forest
- Concept of Bagging explained  
- Compared with Decision Tree  
- Feature Importance plotted  
- RF showed better generalization and reduced overfitting

### 3. Gradient Boosting
- Implemented XGBoost (main model)  
- LightGBM added for learning purpose  
- Compared Boosting vs Bagging  
- XGBoost gave best performance

### 4. Hyperparameter Tuning
- Used:
  - RandomizedSearchCV  
  - GridSearchCV  
- Compared both methods  
- Tuned parameters:  
  - n_estimators  
  - max_depth  
  - learning_rate

### 5. Model Interpretability
- Tree visualization  
- Feature importance  
- SHAP values to explain predictions

---

## Results Summary

| Model | Accuracy |
|------|---------|
| Decision Tree | ~0.80 |
| Random Forest | ~0.85 |
| XGBoost | ~0.87 |
| LightGBM | ~0.87 |

- XGBoost selected as final model  
- Boosting outperformed bagging  
- Important features: capital_gain, age, education, marital_status

---

## Libraries Used
- pandas  
- numpy  
- sklearn  
- xgboost  
- lightgbm  
- shap  
- matplotlib
