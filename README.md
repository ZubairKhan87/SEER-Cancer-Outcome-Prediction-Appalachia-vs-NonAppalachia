# SEER-Cancer-Outcome-Prediction-Appalachia-vs-NonAppalachia


This project analyzes cancer outcomes in the **Appalachia** and **Non-Appalachia** regions using the **SEER dataset**. The goal is to identify demographic, clinical, and socio-economic factors influencing outcomes and compare the performance of **Logistic Regression** and **XGBoost** models.

## Key Highlights
- **Objective:** Predict cancer outcomes and compare regional disparities between Appalachia and Non-Appalachia.
- **Dataset:** SEER dataset with demographic, clinical, and socio-economic features.
- **Preprocessing:**
  - Feature selection based on impact on outcomes.
  - Standardization of continuous variables using z-score.
  - Train-test-validation split (70-20-10 ratio).
- **Models:**
  - **Logistic Regression:** Baseline classifier with multiple solvers (e.g., lbfgs, newton-cg, liblinear).
  - **XGBoost:** Handles feature interactions and class imbalance. Hyperparameters tuned using grid search.
- **Performance Metrics:**
  - Accuracy, F1-score, TPR, TNR, PPV, NPV.
  - AUROC scores for both regions (Appalachia: 0.7755, Non-Appalachia: 0.8055).
- **Key Findings:**
  - **XGBoost** outperformed Logistic Regression with **60.17% accuracy** and **58.73% F1-score** on Non-Appalachia data.
  - **Income level** and **education level** were the most significant predictors.
  - Clinical history had a higher impact in the Appalachia region.
- **Tools Used:** Python, Scikit-learn, XGBoost, SHAP for feature importance.

## Future Improvements
- Collect more data for better generalization.
- Experiment with more complex models (e.g., deep learning).
- Incorporate real-world feedback to improve predictions.

## References
- [Logistic Regression](https://www.ibm.com/topics/logistic-regression)
- [XGBoost Documentation](https://xgboost.readthedocs.io/en/stable/)
- [Python](https://www.python.org/)
