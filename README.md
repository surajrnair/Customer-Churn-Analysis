# 📊 Telco Customer Churn Analysis & Prediction

## 🚀 Project Overview

Customer churn is one of the biggest revenue risks for telecom companies. 
This project analyses customer subscription behaviour and builds a predictive model to identify customers at high risk of churn.

The goal is to:
- Understand key drivers of churn
- Build a machine learning model to predict churn
- Provide data-driven retention strategies

---

## 🏢 Business Problem

Telecom companies lose revenue when customers cancel their subscriptions. 
Acquiring new customers is significantly more expensive than retaining existing ones.

By predicting churn early, the company can:
- Launch targeted retention campaigns
- Offer personalised incentives
- Reduce revenue leakage

---

## 📂 Dataset Description

The dataset contains customer-level information including:

- Demographics (Gender, Senior Citizen, Partner, Dependents)
- Subscription details (Contract Type, Internet Service, Phone Service)
- Account information (Tenure, Monthly Charges, Total Charges)
- Payment Method
- Churn Label (Yes / No)
  
Target Variable: `Churn`

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔎 Project Workflow

### 1️⃣ Data Cleaning & Preprocessing
- Converted `TotalCharges` to numeric
- Handled missing values
- Encoded categorical variables using One-Hot Encoding
- Removed potential data leakage features
- Standardised numerical variables

---

### 2️⃣ Exploratory Data Analysis (EDA)

Key patterns identified:

- Customers with month-to-month contracts churn significantly more
- Higher monthly charges correlate with higher churn probability
- Customers with short tenure are more likely to churn
- Electronic check payment method shows higher churn rate

---

### 3️⃣ Feature Engineering

- Created tenure categories
- Normalised charge variables
- Encoded categorical features
- Removed multicollinearity

---

### 4️⃣ Model Building

Two models were evaluated:

- Logistic Regression
- Random Forest Classifier

---

## 📊 Model Performance

### Final Model: Random Forest

| Metric | Score |
|--------|--------|
| Accuracy | 0.78 |
| Precision | 0.6 |
| Recall | 0.472 |
| F1 Score | 0.528 |

Confusion Matrix and ROC Curve visualisations are included in the notebook.

---

## 📈 Feature Importance

Top churn drivers:

- Contract Type (Month-to-month)
- Tenure
- Monthly Charges
- Payment Method (Electronic Check)
- Internet Service Type

---

## 💡 Business Insights

- Month-to-month customers are the highest churn risk group.
- Customers within the first 12 months are most vulnerable.
- Higher pricing without perceived value increases churn probability.
- Long-term contracts significantly reduce churn risk.

---

## 🎯 Business Recommendations

- Introduce loyalty discounts for long-term contracts
- Offer retention incentives for customers in first 12 months
- Provide bundled packages for high monthly charge customers
- Target electronic check users with auto-payment incentives

---

## 🧠 Future Improvements

- Hyperparameter tuning (GridSearchCV)
- Cross-validation
- SMOTE for class imbalance
- Deploy model using Streamlit
- Build Power BI retention dashboard

---

## 📎 Author

Suraj Nair  
Master of Data Science  
Data Analyst | Machine Learning Enthusiast  
