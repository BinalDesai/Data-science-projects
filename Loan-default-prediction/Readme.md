# 💳 Credit Risk Analysis & Loan Default Prediction

## 🎯 Problem Statement
Financial institutions face significant risks when approving loans. This project aims to predict whether a customer will default on a loan using historical data and machine learning techniques. The objective is to **minimize financial risk, improve profitability, and enable data-driven lending decisions**.

---

## 📊 Exploratory Data Analysis

### 📌 Loan Status Distribution (Target Variable)
<img src="Images/churn_distribution.jpg" width="500"/>

- The dataset is **imbalanced**, with significantly more non-defaulters than defaulters  
- Highlights the importance of focusing on **recall and precision**, not just accuracy  

---

### 📌 Credit Score vs Loan Status
<img src="Images/credit_score_vs_loan.jpg" width="500"/>

- Borrowers with **lower credit scores show higher default risk**  
- Credit score is a **critical feature** for predicting loan outcomes  

---

### 📌 Loan Amount Distribution
<img src="Images/loan_amount_distribution.jpg" width="500"/>

- Most loans fall within the **low to mid-range**  
- Distribution is **right-skewed**, with fewer high-value loans  

---

## 🔍 Key Insights from EDA

- Credit-related features strongly influence loan default behavior  
- Dataset imbalance can bias models toward predicting non-defaults  
- Feature relationships (e.g., credit score, income) are important for risk prediction  

---

## 🤖 Models Used

- Logistic Regression  
- Random Forest  
- Gradient Boosting  

---

## 📊 Model Comparison

### 🔹 Logistic Regression
- Accuracy: **79%**  
- Precision: **67.97%**  
- Recall: **12%** ❌  

👉 Performs well on overall accuracy but **fails to detect defaulters effectively**  
👉 High number of **false negatives** → risky for business use  

---

### 🔹 Random Forest
- Accuracy: **92.87%**  
- Precision: **88.99%**  
- Recall: **77.66%**  

👉 Strong performance with **good balance** between precision and recall  
👉 Significantly improves detection of high-risk customers  

---

### 🔹 Gradient Boosting (Best Model) 🏆
- Accuracy: **93.17%**  
- Precision: **88.99%**  
- Recall: **79.20%**  

👉 Best overall performance  
👉 Highest recall → **better at identifying defaulters**  
👉 Minimizes false negatives → **critical for financial risk management**  

---

## 🏆 Best Performing Model: Gradient Boosting

Gradient Boosting outperformed all other models by achieving the highest accuracy and recall.  
Since **recall is crucial in loan default prediction** (to avoid missing high-risk applicants), this model is the most suitable for real-world deployment.

---

## 📊 Model Performance

### 📌 Confusion Matrix
<img src="Images/confusion_matrix.png" width="500"/>

- Correctly identified **1592 defaulters**  
- Missed only **418 defaulters** (lowest among models)  
- Demonstrates strong predictive performance and reliability  

---

## 💼 Business Impact

- Identifies **high-risk loan applicants early**  
- Reduces **loan defaults and financial losses**  
- Supports **data-driven lending decisions**  
- Improves **customer experience with faster and smarter approvals**  

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy)  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## ⚙️ How to Run

1. Clone the repository  
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open and run the notebook  

---

## 💡 Key Learnings

- Importance of handling **imbalanced datasets**  
- Why **recall is more critical than accuracy** in risk-based problems  
- Comparison and evaluation of multiple ML models  
- How **boosting techniques improve predictive performance**  

---

## 🚀 Future Improvements

- Apply advanced models like **XGBoost or LightGBM**  
- Perform **hyperparameter tuning** for optimization  
- Use **feature engineering** to improve model performance  
- Deploy model using a **web app or dashboard**  

---

⭐ This project demonstrates end-to-end data analysis and machine learning applied to a real-world financial problem.
