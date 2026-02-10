# 📈 Online Retail Sales Forecasting & Tableau Dashboards (ML + Tableau)

🔗 **Live Exploratory Tableau Dashboard:**  
https://public.tableau.com/shared/X8JPHBQY5?:display_count=n&:origin=viz_share_link

End-to-end sales analytics and forecasting project using **Python (Machine Learning)** and **Tableau**, based on the **UK Online Retail dataset**.

The project combines:

* **Exploratory business intelligence in Tableau**, and
* **Predictive analytics using machine learning**,

to support data-driven decision-making in an e-commerce context.

---

## 🧭 Business Context

This project is based on the **Online Retail (UK) dataset**, which contains real transactional data from a UK-based online store between **December 2010 and December 2011**.

The dataset includes:

* Invoice number and date
* Product description
* Quantity and unit price
* Customer ID
* Country

The dataset is realistic and messy, including:

* Cancelled orders (negative quantities)
* Missing customer IDs
* Price outliers

These issues were addressed during data cleaning and exploratory analysis.

---

## 🎯 Project Objective

The main business question of this project is:

> **How can we forecast monthly revenue and evaluate different commercial scenarios in an e-commerce business?**

To answer this, the project follows a two-stage analytical approach:

1️⃣ **Exploratory analysis with Tableau (descriptive analytics)**
2️⃣ **Machine learning forecasting with Python + predictive Tableau dashboard**

This workflow reflects real industry practice: first understand the data visually, then model it.

---

## 🛠 Tools & Technologies

* **Python:** Pandas, NumPy, Scikit-learn, Matplotlib
* **Machine Learning:** Regression models, time-based validation
* **Visualization:** Tableau Desktop / Tableau Public
* **Version Control:** Git & GitHub

---

## 🔍 Stage 1 — Data Preparation & Exploratory Data Analisis (EDA) 


* Data cleaning and validation
* Removal of cancelled transactions
* Monthly aggregation by country
* Revenue calculation:

> `Revenue = Quantity × UnitPrice`


---

## 🔍 Stage 2 Exploratory Tableau Dashboard (First Dashboard)


Before building any machine learning model, an exploratory Tableau dashboard was created to understand historical sales behavior and business patterns.

This dashboard aimed to:

* Explore historical trends visually
* Identify seasonality and anomalies
* Generate business hypotheses
* Inform feature engineering decisions for the ML model

The exploratory dashboard contains:

1️⃣ **Monthly Revenue Trend**

* Shows overall sales evolution from Dec 2009 to Dec 2011
* Helps detect seasonality and growth patterns

2️⃣ **Revenue by Country**

* Highlights the most important markets
* Shows strong revenue concentration in a few countries (mainly the UK, Germany, and France)

3️⃣ **Top Products by Revenue**

* Identifies best-selling products
* Useful for inventory and marketing prioritization

4️⃣ **Customer Contribution Analysis**

* Reveals that a small number of customers generate a large share of revenue (Pareto effect)


🔗 **Access it here:**  
https://public.tableau.com/shared/X8JPHBQY5?:display_count=n&:origin=viz_share_link

📷 **Dashboard Preview:**

![Exploratory Tableau Dashboard](images/exploratory_dashboard.png)

👉 This dashboard provided the analytical foundation that guided the feature engineering and forecasting strategy.

---

## 🧠 Stage 3 — Machine Learning Methodology


### 1️⃣ Feature Engineering

New features were created to improve forecasting:

* Temporal features (year, month)
* Lagged revenue features
* Rolling averages (3-month and 6-month)

---

### 2️⃣ Modeling & Forecasting

* Time-based train/test split

* Baseline model: previous month revenue

* Regression-based machine learning model

* Evaluation using:

  * MAE
  * RMSE
  * MAPE

* Short-term revenue forecast for future months

---

## 🔮 Forecasting Strategy

* **Training period:** Dec 2009 – Sep 2011
* **Validation period:** Oct 2011 – Nov 2011
* **Forecast horizon:** Dec 2011 – Feb 2012

Historical predictions were compared against real data, while future predictions were presented as scenarios rather than exact values.

---

## 📊 Stage 4 — Predictive Tableau Dashboards

The final Tableau workbook includes four main views:

### ✅ Executive Overview

* KPIs
* Revenue trends
* High-level business insights

### ✅ Forecast Analysis

* Real vs predicted revenue
* Error analysis over time

### ✅ What-If Scenarios

Interactive parameters allowing users to simulate:

* Revenue growth
* Changes in number of customers
* Changes in average order value

### ✅ Tableau Story

A guided narrative designed for business stakeholders, explaining insights step-by-step.

---

## 🗂️ Project Structure

```text
online-retail-forecast-tableau/
│
├── data/
│   ├── raw/
│   │   └── online_retail.xlsx
│   └── processed/
│       ├── monthly_revenue.csv
│       └── monthly_revenue_forecast.csv
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_feature_engineering.ipynb
│   └── 03_modeling.ipynb
│
├── tableau/
│   └── exploratory_dashboard.twb
│   └── revenue_forecast.twb
│
├── images/
│   └── exploratory_dashboard.png
│   └── revenue_forecast.png
│
└── README.md
```

---

## 📌 Key Takeaways

* Demonstrates a **complete end-to-end analytics workflow**
* Combines **machine learning with business visualization**
* Emphasizes interpretability and decision support
* Designed for both technical and non-technical audiences
* Shows professional data science best practices

---

## 👤 Author

**Nahuel Moreno Yalet**
Industrial Engineer | PhD in Theoretical & Computational Chemistry
Data Analyst | Data Scientist
SQL • Python • Tableau • Power BI
