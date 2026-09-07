# 📉 Telecom Customer Churn Prediction 

## 📌 Project Overview

Customer churn is a major challenge for telecom companies, as retaining existing customers is often more cost-effective than acquiring new customers.

This project focuses on building Machine Learning models to predict whether a **high-value telecom customer is likely to churn in the near future**. The project also identifies important variables influencing customer churn and provides data-driven insights to support customer retention strategies.

---

## 🎯 Business Objective

The primary objectives of this project are to:

* Predict whether a high-value customer is likely to churn in the near future.
* Identify the key variables that are strong predictors of customer churn.
* Compare different Machine Learning models and feature selection techniques.
* Evaluate models using Accuracy, Precision, Recall, and ROC-AUC scores.
* Recommend strategies to help telecom companies manage and reduce customer churn.

---

## 📊 Dataset

The dataset contains customer-level telecom usage and service information collected across multiple months.

The analysis focuses on identifying **high-value customers** and predicting whether they are likely to churn based on their usage patterns and customer behavior.

**Dataset Source:** Kaggle – Telecom Churn Case Study Hackathon

[View Dataset on Kaggle](https://www.kaggle.com/competitions/telecom-churn-case-study-hackathon-c35?utm_source=chatgpt.com)

---

## 🛠️ Project Workflow

The project follows an end-to-end Machine Learning workflow:

### 1️⃣ Data Understanding

* Dataset inspection
* Understanding features and data types
* Missing value analysis
* Duplicate record detection
* Target variable analysis
* Customer churn distribution analysis

### 2️⃣ Data Cleaning

* Handling missing values
* Removing unnecessary features
* Correcting data types
* Identifying potential data leakage
* Preparing the dataset for Machine Learning

### 3️⃣ Exploratory Data Analysis (EDA)

The analysis explores:

* Customer churn distribution
* Customer usage behavior
* Revenue and recharge patterns
* Telecom service usage
* Important features associated with customer churn

### 4️⃣ Feature Engineering & Selection

Different techniques were used to reduce dimensionality and identify important features:

* Principal Component Analysis (PCA)
* Recursive Feature Elimination (RFE)
* Feature importance using Random Forest

### 5️⃣ Machine Learning Models

The following model combinations were developed and evaluated:

* PCA + XGBoost Classifier
* PCA + Random Forest Classifier
* RFE (Random Forest) + Random Forest Classifier

---

## 📈 Model Evaluation

The models were evaluated using multiple performance metrics:

| Metric        | Description                                                      |
| ------------- | ---------------------------------------------------------------- |
| Accuracy      | Percentage of total predictions that are correct                 |
| Precision     | Percentage of predicted churners who actually churned            |
| Recall        | Percentage of actual churners correctly identified               |
| ROC-AUC Score | Model's ability to distinguish between churners and non-churners |

---

## 🏆 Model Results

The following results represent the current version of the project.

### PCA + XGBoost

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 0.9209 |
| Precision | 0.6551 |
| Recall    | 0.4325 |
| ROC-AUC   | 0.7037 |

### PCA + Random Forest

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 0.9173 |
| Precision | 0.6863 |
| Recall    | 0.3096 |
| ROC-AUC   | 0.6470 |

### RFE (Random Forest) + Random Forest

| Metric    |      Score |
| --------- | ---------: |
| Accuracy  | **0.9429** |
| Precision | **0.7863** |
| Recall    | **0.5841** |
| ROC-AUC   | **0.7833** |

---

## 📊 Model Comparison

| Model                   |   Accuracy |  Precision |     Recall |    ROC-AUC |
| ----------------------- | ---------: | ---------: | ---------: | ---------: |
| PCA + XGBoost           |     0.9209 |     0.6551 |     0.4325 |     0.7037 |
| PCA + Random Forest     |     0.9173 |     0.6863 |     0.3096 |     0.6470 |
| **RFE + Random Forest** | **0.9429** | **0.7863** | **0.5841** | **0.7833** |

### Best Performing Model

Based on the current evaluation results:

**RFE (Random Forest) + Random Forest Classifier** achieved the best overall performance.

* **Accuracy:** 94.29%
* **Precision:** 78.63%
* **Recall:** 58.41%
* **ROC-AUC:** 78.33%

> These results will be re-evaluated and updated as the Machine Learning pipeline is improved.

---

## 🔍 Key Insights

The analysis helps identify:

* Important variables that influence customer churn.
* High-value customers who may be at risk of leaving.
* Customer usage patterns associated with churn.
* Features that can be used to support early churn prediction.

---

## 💡 Business Recommendations

Based on the customer churn analysis, telecom companies can:

* Identify high-value customers with a high probability of churn.
* Develop targeted retention campaigns for at-risk customers.
* Offer personalized recharge plans and incentives.
* Monitor significant changes in customer usage patterns.
* Improve customer service for high-risk customer segments.
* Prioritize retention strategies based on churn probability.

---

## 📂 Project Structure

```text
Telecom-Churn-Case-Study/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── Telecom_Churn_Case_Study.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🧰 Technologies Used

### Programming Language

* Python 3.9

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost

### Development Environment

* Anaconda
* Jupyter Notebook

---

## 🚀 Future Improvements

The project will be further improved by:

* Rebuilding the Machine Learning pipeline with proper preprocessing.
* Using stratified train-test splitting.
* Implementing cross-validation.
* Correctly calculating ROC-AUC using predicted probabilities.
* Handling class imbalance.
* Performing hyperparameter tuning.
* Comparing additional Machine Learning models.
* Optimizing the decision threshold.
* Updating and validating the final model metrics.

---

## 👤 Author

**Tejesh Guntu**

⭐ If you found this project interesting, feel free to star the repository!
