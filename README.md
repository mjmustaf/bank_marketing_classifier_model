
# Bank Marketing Classifier Comparison

This repository contains a Jupyter Notebook that compares the performance of several machine learning classifiers using a dataset related to the marketing of term deposit products by a Portuguese bank. The project focuses on building, evaluating, and improving classification models to predict whether a customer will subscribe to a term deposit.

---

##  Jupyter Notebook

[Maketing Jupyter Notebook](bank_marketing_classifier_comparison.ipynb)

---

##  Summary of Findings

- **Business Objective**: Predict if a client will subscribe to a term deposit after a telemarketing campaign.
- **Dataset**: Sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing), includes client demographics, economic indicators, and campaign interaction history.
- **Target Variable**: `y` (binary: `yes` or `no` for term deposit subscription)

###  Models Used
- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Support Vector Machine

###  Modeling & Evaluation
- All models were trained with default settings and evaluated using accuracy and F1-score.
- GridSearchCV was applied to optimize hyperparameters.
- Logistic Regression with `class_weight='balanced'` improved the F1-score from **0.34** to **0.4593**, significantly improving recall on the minority class.

---

## Visualizations

- Descriptive statistics and distributions for continuous and categorical variables
- Seaborn and matplotlib used for clean, well-labeled plots
- Subplots and scaling used where appropriate

---

##  Data Cleaning & Preparation

- Dropped the `duration` column (not suitable for real-time prediction)
- Handled missing values labeled as "unknown"
- Used one-hot encoding for categorical variables
- Split dataset using stratified train/test split (80/20)

---

##  Recommendations

- Use **Logistic Regression with class weighting** or a **tuned Decision Tree** for production


