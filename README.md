# Data Science & Analytics – Task 2 (2026)
### Customer Retention & Churn Analysis
**Future Interns – Data Science & Analytics Internship**

## 📌 About the Task

This project analyzes real-world telecom customer data to understand churn behavior and answer key business questions:

- Why are customers leaving the platform?
- Which customer segments are most likely to churn?
- How long do customers typically stay active?
- What actions can improve customer retention?

## 📂 Dataset

**Telco Customer Churn Dataset** (Kaggle)
[https://www.kaggle.com/datasets/blastchar/telco-customer-churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

7,043 customer records including demographics, account information, subscribed services, billing details, and churn status.

## 🛠️ Tools Used

- **Python** – Pandas, Matplotlib, Seaborn
- **Jupyter Notebook** (VS Code)
- **HTML/JS (Chart.js)** – interactive dashboard

## 🧹 Data Cleaning

- Dropped the `customerID` column (not useful for analysis)
- Converted `TotalCharges` from text to numeric and removed rows that failed conversion (11 rows with blank values)
- Created a `Churn_Flag` column (1 = Yes, 0 = No) for numeric analysis
- Final cleaned dataset: 7,032 customers

## 📊 Analysis Performed

- Overall churn rate
- Churn rate by contract type
- Churn rate by tenure (customer lifetime)
- Churn rate by internet service type
- Churn rate by Tech Support and Online Security
- Churn rate by payment method
- Monthly charges comparison: churned vs retained customers

## 💡 Key Insights

1. **Contract type is the biggest churn driver** — Month-to-month customers churn at 42.7%, versus 11.3% on one-year and just 2.8% on two-year contracts.
2. **Churn happens early** — Customers in their first 6 months churn at 53%, dropping below 10% after 4 years of tenure.
3. **Fiber optic and pricing** — Fiber optic customers churn at 41.9% (vs 19% for DSL), and churned customers pay a higher median monthly bill ($79.6 vs $64.4).
4. **Support services retain customers** — Customers without Tech Support or Online Security churn at ~42%, compared to ~15% for those who have them.
5. **Payment method matters** — Electronic check users churn at 45.3%, the highest of any payment method.

## ✅ Recommendations

- Incentivize month-to-month customers to move onto 1-year or 2-year contracts
- Build an onboarding and check-in program for the first 3–6 months, when churn risk is highest
- Investigate fiber optic pricing and service quality
- Bundle Tech Support and Online Security for new customers, especially on fiber plans
- Encourage customers to switch from electronic check to automatic payment methods
- Flag high-bill, month-to-month customers as an at-risk segment for proactive retention offers

## 📁 Repository Contents

| File | Description |
|---|---|
| `Data_set.csv` | Raw telecom customer churn dataset |
| `Task2_Churn_Analysis.ipynb` | Jupyter notebook — data cleaning, analysis & visualizations |
| `Task2_Churn_Analysis.html` | Exported notebook report (charts + insights) |
| `churn_dashboard.html` | Interactive churn dashboard (KPIs + charts) |
| `Screenshots/` | Dashboard preview images |
| `README.md` | Project overview |

## 🚀 How to View

- **Notebook:** open `Task2_Churn_Analysis.ipynb` in Jupyter/VS Code
- **Report:** open `Task2_Churn_Analysis.html` in any browser
- **Dashboard:** open `churn_dashboard.html` in any browser for an interactive view

---
*Submitted as part of the Future Interns Data Science & Analytics internship — Task 2.*
