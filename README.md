# Flipkart CSAT Prediction Project

## Project Overview

This project aims to predict customer satisfaction (CSAT) scores for Flipkart customer support interactions using machine learning. The solution leverages advanced models and feature engineering to help identify dissatisfied customers and improve overall service quality.

---

## Dataset

- **Source:** Customer support data from Flipkart (see `Customer_support_data.csv`)
- **Features:** Channel, category, sub-category, customer remarks, product details, agent shift, sentiment analysis, and more.
- **Target:** CSAT Score (1 to 5)

---

## Approach

1. **Data Preprocessing:**  
   - Handled missing values, encoded categorical variables, and engineered new features (e.g., sentiment scores, interaction duration).

2. **Modeling:**  
   - Compared multiple ML models: Random Forest, Logistic Regression, and XGBoost.
   - Used cross-validation and hyperparameter tuning for optimal performance.
   - Addressed class imbalance with sample weighting.

3. **Evaluation:**  
   - Assessed models using accuracy, precision, recall, F1-score, and multiclass ROC-AUC.
   - Visualized results with confusion matrices and per-class metric plots.

---

## Final Model

- **Selected Model:** XGBoost Classifier
- **Best Parameters:**  
  `{'learning_rate': 0.1, 'max_depth': 9, 'min_child_weight': 1, 'n_estimators': 150, 'subsample': 0.8}`
- **Test Accuracy:** 0.80
- **Macro ROC-AUC:** 0.84

---

## Business Impact

- The model enables proactive identification of dissatisfied customers, allowing targeted interventions.
- High accuracy for the most important classes ensures reliable reporting and actionable insights for customer experience management.

---

## How to Run

1. Clone the repository.
2. Install requirements:  
   `pip install -r requirements.txt`
3. Run the Jupyter notebook or Python script for training and evaluation.
4. The best model is saved as `best_xgb_model.pkl` for easy deployment.

---

## Conclusion

XGBoost provides a robust and accurate solution for CSAT prediction, with strong business value in identifying both highly satisfied and dissatisfied customers. The approach is ready for deployment and further enhancement.

---
