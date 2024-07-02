# Bank Marketing Campaign Classifier

This repository contains a machine learning project aimed at predicting whether clients of a Portuguese bank will subscribe to a term deposit based on various features from previous marketing campaigns.

## Dataset

The dataset used in this project is from marketing campaigns of a Portuguese bank. It includes a variety of features such as:

- **Numerical Features**: `age`, `campaign`, `pdays`, `previous`, `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`
- **Categorical Features**: `job`, `marital`, `education`, `default`, `housing`, `loan`, `contact`, `month`, `day_of_week`, `poutcome`

## Objective

The goal is to build classifiers that can accurately predict whether or not a client will subscribe to a term deposit (`y` column).

## Project Steps

1. **Data Preprocessing**:
    - Handling categorical and numerical features using `OneHotEncoder` and `ColumnTransformer`.
    - Removing features that could lead to data leakage (`duration`).

2. **Model Training and Tuning**:
    - Implementing multiple models: Logistic Regression, Decision Tree, Random Forest, and XGBoost.
    - Using `GridSearchCV` for hyperparameter tuning to find the best parameters for each model.

3. **Model Evaluation**:
    - Assessing model performance using accuracy, classification reports, and other relevant metrics.
    - Interpreting model results using `eli5` for white-box models and `LIME` for local explanations of black-box models.

## Key Results

- **Logistic Regression**: Achieved an accuracy of approximately 82.76% with the best hyperparameters.
- **Decision Tree**: Tuned for optimal depth and minimum samples split.
- **Random Forest**: Optimized for depth and minimum samples split to enhance performance.
- **XGBoost**: Fine-tuned for maximum depth, child weight, and number of estimators.

## Tools and Libraries

- **Python**: Data manipulation and model building.
- **Pandas**: Data processing and handling.
- **Scikit-Learn**: Model building, preprocessing, and evaluation.
- **XGBoost**: Advanced model building.
- **ELI5**: Model interpretation.
- **LIME**: Local interpretable model-agnostic explanations.

## Conclusion

This project showcases the end-to-end process of building, tuning, and interpreting machine learning models to solve a real-world classification problem. The use of various models and interpretation tools highlights the importance of understanding model decisions and ensuring the robustness of predictions.


