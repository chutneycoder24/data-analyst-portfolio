# 📊 Customer Churn Prediction

## 📌 Project Overview
Telecommunication companies often face high customer churn rates, which directly impact revenue.
This project analyzes the **Telco Customer Churn dataset** to predict churn and identify the most important factors influencing customer retention.

---

## 🔧 Tools & Methods
- **Data Cleaning & Wrangling**: Python (pandas, numpy)
- **Exploratory Data Analysis (EDA)**: Matplotlib, Seaborn
- **Modeling**: CART (Classification and Regression Trees), Logistic Regression
- **Visualization**: Tableau dashboard (customer segments & churn rates)

---

## 📊 Key Steps
1. **Data Preparation**
   - Clean missing values in `TotalCharges`.
   - Encode categorical variables (contract type, payment method, etc.).

2. **Exploratory Data Analysis**
   - Customers on month-to-month contracts are **3x more likely to churn**.
   - High monthly charges strongly correlate with churn probability.

3. **Modeling**
   - **CART Model** achieved ~82% accuracy.
   - Logistic Regression achieved ~80% accuracy.
   - CART provided interpretable decision rules (great for business teams).

4. **Visualization**
   - Tableau dashboard showing churn distribution by contract type, charges, and tenure.

---

## 📈 Results & Business Recommendations
- Customers with **month-to-month contracts** and **high monthly charges** are at highest churn risk.
- Recommendation:
  - Offer discounts for long-term contracts.
  - Target retention campaigns at high-charge, short-tenure customers.

---

## 📂 Structure
- `data/` → raw + cleaned dataset
- `notebooks/` → cleaning, EDA, modeling
- `reports/` → case study (PDF/Markdown)
- `visuals/` → decision tree, confusion matrix, screenshots

---

## 🔗 Links
- Notebook: `notebooks/03_modeling_CART.ipynb` (placeholder)
- Dashboard: *(add your Tableau link)*
- Report: `reports/churn_case_study.md`
