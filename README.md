# 📈 Online Retail Sales Forecasting & Tableau Dashboard

End-to-end sales forecasting project using **Python (Machine Learning)** and **Tableau**, based on the **UK Online Retail dataset**.  
The project focuses on predicting future revenue and communicating insights through interactive dashboards and business-oriented storytelling.

---

## 🎯 Business Objective

The goal of this project is to answer the following question:

> **How can we forecast monthly revenue and evaluate different commercial scenarios in an e-commerce business?**

Using historical transaction data, a machine learning model is trained to predict future sales, and the results are visualized in Tableau to support decision-making.

---

## 📦 Dataset

**Source:** Online Retail (UK) dataset  
**Period:** December 2010 – December 2011  

The dataset contains transactional data from a UK-based online retailer, including:

- Invoice number and date  
- Product information  
- Quantity and unit price  
- Customer ID  
- Country  

> ⚠️ The dataset includes cancelled orders (negative quantities), missing customer IDs, and price outliers, which are handled during data cleaning and EDA.

---

## 🧠 Methodology

### 1️⃣ Data Preparation & EDA
- Data cleaning and validation
- Removal of cancelled transactions
- Revenue calculation (`Quantity × UnitPrice`)
- Monthly aggregation by country
- Exploratory analysis focused on business metrics

### 2️⃣ Feature Engineering
- Temporal features (year, month)
- Lagged revenue features
- Rolling averages (3M, 6M)
- Business metrics:
  - Number of orders
  - Unique customers
  - Average order value

### 3️⃣ Modeling & Forecasting
- Time-based train / test split
- Baseline model (previous month revenue)
- Machine learning model (regression-based)
- Evaluation using MAE, RMSE, and MAPE
- Short-term revenue forecast for future months

### 4️⃣ Visualization & Storytelling (Tableau)
- Real vs predicted revenue analysis
- Forecast visualization with clear temporal separation
- What-if scenarios using interactive parameters
- Executive-level storytelling using Tableau Story Points

---

## 🔮 Forecasting Strategy

- **Training period:** Dec 2010 – Sep 2011  
- **Validation period:** Oct 2011 – Nov 2011  
- **Forecast horizon:** Dec 2011 – Feb 2012  

Historical predictions are evaluated against real data, while future predictions are presented as scenarios rather than exact values.

---

## 📊 Tableau Dashboards

The Tableau workbook includes:

- **Executive Overview:** KPIs and revenue trends  
- **Forecast Analysis:** Real vs predicted revenue and error analysis  
- **What-If Scenarios:** Impact of growth and customer changes  
- **Story:** Guided narrative for business stakeholders  

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
│   └── revenue_forecast.twbx
│
├── images/
│   └── dashboard_preview.png
│
└── README.md

---


🛠️ Tools & Technologies

Python: Pandas, NumPy, Scikit-learn, Matplotlib

Machine Learning: Regression models, time-based validation

Visualization: Tableau

Version Control: Git & GitHub

📌 Key Takeaways

Demonstrates an end-to-end analytics workflow

Combines machine learning with business-focused visualization

Emphasizes interpretability and decision support

Designed to be understandable for both technical and non-technical stakeholders

👤 Author

Nahuel Moreno Yalet
Industrial Engineer | PhD in Theoretical & Computational Chemistry
Data Analytics & Data Scientist
