📊 Customer Churn Prediction
📌 Project Overview

Telecommunication companies face significant revenue loss from customer churn. This project analyzes the Telco Customer Churn dataset to:

Predict customer churn.

Identify the main factors driving attrition.

Provide business recommendations to improve retention.

📂 Project Structure
flagship-project-churn/
│
├── data/                # raw and cleaned datasets
├── notebooks/           # Jupyter notebooks (EDA, modeling, evaluation)
├── reports/             # case study report (Markdown + PDF)
├── visuals/             # decision tree, confusion matrix, dashboard
└── README.md            # project overview


🔧 Tools & Methods

Data Cleaning & Wrangling: Python (pandas, numpy)

Exploratory Data Analysis (EDA): matplotlib, seaborn

Modeling: CART (Classification and Regression Tree), Logistic Regression

Visualization: Tableau / Power BI (dashboards), static PNGs

📊 Key Steps

Data Preparation

Cleaned missing values in TotalCharges.

Encoded categorical variables.

Balanced dataset (churn ≈ 26%).

Exploratory Data Analysis (EDA)

Month-to-month customers had the highest churn (~43%).

High monthly charges strongly correlated with churn.

Tenure under 1 year was the riskiest group.

Modeling

CART: ~82% accuracy. Provided clear business rules.

Logistic Regression: ~80% accuracy. Confirmed variable significance.

📈 Results & Insights

Top Predictors of Churn:

Contract type (month-to-month most at risk).

Monthly charges (higher bills → higher churn).

Customer tenure (shorter tenure → higher churn).

Business Recommendations:

Promote 1–2 year contracts with discounts.

Launch retention campaigns for short-tenure, high-charge customers.

Offer bundles/loyalty perks to reduce bill shock.

📑 Report

Case Study (Markdown)

Case Study (PDF)

🖼 Visuals
CART Decision Tree

Confusion Matrix

Sample Dashboard
