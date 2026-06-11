Dataset used from Kaggle: https://www.kaggle.com/datasets/algozee/teenager-menthal-healy. This project is for educational purposes only.

# Predicting Teen Depression Risk with Machine Learning

## Overview

This project builds a machine learning pipeline to predict whether a teenager may be at risk of depression based on behavioral and lifestyle factors such as social media usage, sleep duration, stress, and anxiety levels.

The goal is to identify patterns in behavior that may be associated with higher risk using supervised learning models.

---
## Tools Used
- Python
- Pandas
- Scikit-learn
- Matplotlib

---

## Models Tested
- Logistic Regression
- K-Nearest Neighbors (KNN)

---

## Problem Type

* **Task:** Supervised Learning
* **Type:** Binary Classification
* **Target:** Depression risk (0 = Not at risk, 1 = At risk)

---

## Dataset

* **Source:** https://www.kaggle.com/datasets/algozee/teenager-menthal-healy
* **Size:** ~1,200 rows × 13 columns
* Includes numerical and categorical features such as age, sleep, stress, anxiety, and social media usage.

---

## Approach

* Performed train-test split before preprocessing to prevent data leakage
* Used a `ColumnTransformer` pipeline:

  * Numerical: imputation + standard scaling
  * Categorical: one-hot encoding
* Built and compared two models:

  * K-Nearest Neighbors (KNN)
  * Logistic Regression
* Used cross-validation and GridSearchCV for model selection and tuning

---

## Results

* Dataset was highly imbalanced, making accuracy alone misleading
* Final model prioritized recall to better identify at-risk individuals

**Logistic Regression (final model):**

* Accuracy: ~97%
* Recall: ~83%
* Precision: ~56%

---

## Key Takeaways

* Anxiety and stress were strong indicators of depression risk
* Higher social media use combined with lower sleep was associated with higher risk
* Logistic Regression provided the best balance of performance and interpretability

## Files
- TeenDepressionPrediction_Notebook.ipynb
- TeenDepressionPredictionProject.pdf

