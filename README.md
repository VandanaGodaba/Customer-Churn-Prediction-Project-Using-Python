# 📊 Customer Churn Prediction using Machine Learning

## 📌 Project Overview
Customer churn refers to customers leaving a company and switching to competitors. In industries like telecommunications, churn directly impacts revenue and customer growth. This project focuses on building a predictive analytics solution to identify customers who are likely to churn, enabling businesses to take proactive retention actions.

Using historical customer data, exploratory data analysis (EDA), feature engineering, and machine learning models, this project predicts churn and identifies key factors influencing customer behavior.

---

## 🎯 Problem Statement
The objective of this project is to analyze customer behavior and build a machine learning model that can accurately predict customer churn. By identifying churn-prone customers early, businesses can reduce customer loss, improve customer satisfaction, and increase long-term profitability.

---

## 📂 Dataset Description
The project uses the **Telco Customer Churn Dataset**, which contains customer demographics, service usage details, billing information, and churn status.

### Key Features:
- Customer demographics (gender, senior citizen, dependents)
- Account information (tenure, contract type, payment method)
- Service usage (internet services, streaming, tech support)
- Billing details (monthly charges, total charges)
- Target variable: **Churn (Yes / No)**

---

## 🔧 Project Workflow

### 🔹 Activity 1: Dataset Familiarization
- Understanding dataset structure and variables
- Identifying target and feature columns

### 🔹 Activity 2: Data Quality Check & Preprocessing
- Checked for missing values and duplicates
- Identified categorical and numerical features
- Converted data types (TotalCharges to numeric)
- Encoding categorical variables
- Normalized numerical features using Min-Max Scaling

### 🔹 Activity 3: Data Cleaning & Exploratory Data Analysis (EDA)
#### Univariate Analysis:
- Analyzed individual variables like tenure, charges, contract type, payment method
- Used histograms and bar charts to understand distributions

#### Bivariate Analysis:
- Studied relationship between features and churn
- Analyzed churn patterns based on contract type, payment method, tenure, and charges

---

## ⚙️ Feature Engineering
- Removed irrelevant columns (customerID)
- Created meaningful features such as:
  - AverageMonthlySpend
  - Contract Type (encoded)
- Used already encoded dataset for modeling
- Ensured no missing values before training

---

## 🤖 Machine Learning Models Used

### Baseline Model:
- **Logistic Regression**

### Advanced Models:
- Decision Tree
- Random Forest

### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1-Score
- AUC-ROC
- Confusion Matrix

---

## 📈 Model Performance Summary

- Logistic Regression achieved the best balance between **Recall** and **AUC-ROC**
- Random Forest performed well but did not significantly outperform Logistic Regression
- Recall for churn customers (Class = 1) was prioritized, as missing churn customers leads to revenue loss

---

## 🏆 Final Model Selection
**Logistic Regression** was selected as the final model because:
- It provided the highest recall for churn customers
- Achieved strong AUC-ROC score
- Easy to interpret for business decision-making
- Performs competitively compared to complex models

---

## 💡 Business Insights
- Customers on month-to-month contracts are more likely to churn
- High monthly charges increase churn risk
- Customers using electronic check payment show higher churn
- Long-term contracts and automatic payment methods reduce churn probability

The model helps businesses identify high-risk customers and take preventive actions such as targeted offers, discounts, and improved customer support.

---

## 📌 Conclusion
This project successfully demonstrates how predictive analytics and machine learning can be applied to solve a real-world business problem. Through effective data preprocessing, feature engineering, and model evaluation, Logistic Regression was identified as the most suitable model for churn prediction.

---

## 🔮 Future Scope
- Hyperparameter tuning for improved performance
- Feature selection and dimensionality reduction
- Cost-sensitive learning to reduce false negatives
- Deployment as a real-time churn prediction system

---

## 🛠 Tools & Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Google Colab
- GitHub

---

## 👩‍💻 Author
**Vandana Godaba**  
Data Analytics & Machine Learning Project

---

⭐ If you found this project useful, feel free to star the repository!
