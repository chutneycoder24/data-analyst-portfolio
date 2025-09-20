# 📊 Customer Churn Prediction Case Study

## 1. Project Overview
Customer churn is a critical issue for telecommunications companies. Losing customers directly reduces revenue and increases acquisition costs.  
This project analyzes the **Telco Customer Churn dataset** (7,043 customers, 21 variables) to:  
- Predict churn likelihood.  
- Identify the key factors driving customer attrition.  
- Recommend strategies to improve retention.  

---

## 2. Dataset
- **Source:** IBM Sample Data / Kaggle (Telco Customer Churn)  
- **Size:** 7,043 rows × 21 columns  
- **Key Features:**  
  - Customer demographics (gender, senior citizen, dependents)  
  - Account information (tenure, contract type, payment method)  
  - Services (internet, phone, streaming)  
  - Charges (MonthlyCharges, TotalCharges)  
- **Target Variable:** `Churn` (Yes/No)

---

## 3. Methodology

### 3.1 Data Preparation
- Cleaned missing values in `TotalCharges`.  
- Converted categorical variables (e.g., `Contract`, `PaymentMethod`) to dummy variables.  
- Balanced dataset with churn ≈ 26%.  

### 3.2 Exploratory Data Analysis
- **Tenure**: Customers with <12 months tenure have highest churn.  
- **Contract**: Month-to-month contracts show ~43% churn, compared to ~11% for 2-year contracts.  
- **Charges**: High monthly charges correlate strongly with churn.  

### 3.3 Modeling
Two models were tested:  
- **CART (Classification and Regression Tree)**  
  - Accuracy: ~82%  
  - Provided clear decision rules (e.g., “If contract=month-to-month and tenure < 12 months → high churn risk”).  
- **Logistic Regression**  
  - Accuracy: ~80%  
  - Helped confirm predictor significance (p-values).  

---

## 4. Results
- **Top Churn Predictors:**  
  1. Contract type (month-to-month is riskiest).  
  2. Monthly charges (higher bills → higher churn).  
  3. Tenure (shorter tenure → higher churn).  

- **Model Comparison:**  
  - CART slightly outperformed logistic regression in accuracy.  
  - CART was easier to explain to non-technical stakeholders.  

---

## 5. Business Recommendations
- **Promote Long-Term Contracts**: Offer discounts for 1–2 year contracts to reduce churn risk.  
- **Customer Retention Campaigns**: Target month-to-month customers with <1 year tenure.  
- **Billing Adjustments**: Consider loyalty discounts or service bundles for high-charge customers.  
- **Proactive Service**: Monitor early-tenure customers closely, provide onboarding support.  

---

## 6. Limitations & Future Work
- Dataset does not include qualitative data (customer satisfaction, reasons for churn).  
- Could integrate time-series retention tracking.  
- Next steps: Try Random Forest / Gradient Boosting for higher predictive accuracy.  

---

## 7. Conclusion
This analysis demonstrates how **data-driven insights** can guide retention strategy. By identifying at-risk customers early, telecom companies can reduce churn, increase lifetime value, and improve profitability.  

**Key Takeaway:** Contract type and customer tenure are the strongest levers for churn management.  

---
