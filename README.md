# MLArena
# 🏦 Loan Approval Prediction — Machine Learning Model Comparison

## 📌 Project Overview

This project presents a comprehensive comparison of multiple machine learning classification models applied to a real-world **Loan Approval dataset**. The goal is to build reliable predictive models that determine whether a loan application should be approved based on applicants’ financial and demographic attributes.

The project demonstrates a complete end-to-end machine learning workflow including data analysis, preprocessing, model training, evaluation, visualization, and performance comparison.

---

## 📊 Dataset

The dataset consists of **2,000 loan applications** with **8 features**, combining financial indicators and demographic information.

### Feature Summary

| Feature          | Description                           |
| ---------------- | ------------------------------------- |
| `name`           | Applicant name                        |
| `city`           | City of residence                     |
| `income`         | Monthly income (USD)                  |
| `credit_score`   | Credit score                          |
| `loan_amount`    | Requested loan amount                 |
| `years_employed` | Years of employment                   |
| `points`         | Financial scoring metric              |
| `loan_approved`  | Target variable (Approved / Rejected) |

* **Problem Type:** Binary Classification
* **Target Variable:** `loan_approved`

---

## 🔍 Exploratory Data Analysis (EDA)

* Verified dataset completeness (no missing values).
* Analyzed class distribution to ensure balance between approved and rejected loans.
* Visualized target distribution using bar plots to validate suitability for supervised learning.

---

## ⚙️ Data Preprocessing Pipeline

To ensure optimal model performance, the following preprocessing steps were applied:

* **Categorical Encoding:**
  Label Encoding for `name` and `city`
* **Feature Scaling:**
  StandardScaler applied to all numerical features
* **Train–Test Split:**
  80% training / 20% testing with stratification to preserve class balance

---

## 🤖 Machine Learning Models Implemented

The following classification models were trained and evaluated:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Random Forest
* Support Vector Machine (SVM)
* Naive Bayes
* Artificial Neural Network (MLPClassifier)
* Gradient Boosting Classifier *(additional model)*

> ⚠️ Decision Trees were intentionally excluded as per assignment constraints.

---

## 📈 Model Evaluation

Each model was evaluated using industry-standard metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### 📊 Performance Comparison

| Model               | Accuracy  | Precision | Recall    | F1-Score  |
| ------------------- | --------- | --------- | --------- | --------- |
| Logistic Regression | **1.000** | **1.000** | **1.000** | **1.000** |
| Random Forest       | **1.000** | **1.000** | **1.000** | **1.000** |
| Gradient Boosting   | **1.000** | **1.000** | **1.000** | **1.000** |
| Naive Bayes         | 0.9625    | 0.9763    | 0.9375    | 0.9565    |
| ANN                 | 0.8675    | 0.7686    | **1.000** | 0.8691    |
| SVM                 | 0.5600    | 0.0000    | 0.0000    | 0.0000    |
| KNN                 | 0.4975    | 0.4252    | 0.4034    | 0.4140    |

Confusion matrices and visualizations were used to interpret model behavior and error patterns.

---

## 🧠 Key Insights

* **Top Performers:** Logistic Regression, Random Forest, and Gradient Boosting achieved perfect classification.
* **Ensemble models** demonstrated superior performance by capturing non-linear relationships and reducing variance.
* **ANN** showed strong recall but lower precision, indicating false positives.
* **Naive Bayes** performed well but was limited by its independence assumptions.
* **KNN and SVM** underperformed, highlighting sensitivity to hyperparameters and feature distribution.

---

## 💡 Discussion

* Perfect Logistic Regression performance suggests linear separability in the scaled feature space.
* Ensemble methods proved robust and reliable for loan approval prediction.
* Neural networks require careful tuning to outperform traditional models.
* Proper preprocessing and scaling were critical for model success.

---

## ✅ Conclusion

This project successfully demonstrates how different machine learning models perform on a loan approval prediction task. Through systematic preprocessing, evaluation, and comparison, the most effective models were identified, highlighting the importance of model selection and data preparation in real-world machine learning applications.

---

## 📁 Repository Contents

* `notebook.ipynb` — Complete implementation and visualizations
* `report.pdf` — Detailed project report
* `README.md` — Project overview and documentation

---

## 🚀 Skills Demonstrated

* Data preprocessing & feature engineering
* Supervised machine learning
* Model evaluation & comparison
* Data visualization
* Practical ML decision-making


