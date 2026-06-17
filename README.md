# Bank Customer Churn Analysis

## Overview
This project analyses a dataset of 10,000 bank customers to identify 
Why do customers churn, and predict which customers are likely to leave? 
Using SQL, I uncovered key churn patterns and visualised findings with 
Python, and built a Logistic Regression model that predicts customer 
Churn with 81.6% accuracy.

**Tools used:** SQL (SQLite) · Python · Pandas · Matplotlib · Scikit-learn

**Data source:** [Bank Customer Churn Dataset — Kaggle](https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction)

---

## Key Findings
-  **Germany** churns at 32% — double the rate of France and Spain (16%)
-  Customers with **4 products** have a **100% churn rate** — the bank is overselling
-  Customers aged **46-60** are the highest risk group at **51% churn**
-  **Logistic Regression model** achieves **81.6% accuracy** predicting churn
-  **IsActiveMember** is the strongest predictor of churn according to the model

---

## Business Recommendations

**1. Investigate Germany urgently**
Germany churns at 32% — double France and Spain. With 2,509 German customers, reducing churn to match other markets would retain ~413 additional customers annually, worth approximately £200,000+ in preserved revenue. Root cause investigation recommended — pricing, product fit, or local competition may be driving this.

**2. Cap cross-selling at 2 products**
Customers with 4 products churn at 100% and 3 products at 83%. The sweet spot is 2 products at just 7.6% churn. The bank should immediately audit customers holding 3-4 products and implement a cross-selling cap to protect retention.

**3. Target the 46-60 age segment**
Over half of middle-aged customers (51%) churn — the highest of any group. A targeted retention campaign for this segment — loyalty rewards, personalised financial products, or dedicated relationship managers — could significantly reduce overall churn.

**4. Re-evaluate active membership definition**
The model identifies IsActiveMember as the strongest churn predictor, yet SQL analysis shows active and inactive members churn at almost the same rate (20.8% vs 20.2%). This suggests the current definition of "active" may not reflect genuine engagement — the bank should redefine what active membership means.

---

## Project Structure
- `churn_analysis.sql` — SQL queries analysing churn by geography, age, products, and activity
- `Bank_Customer_Churn_Analysis.ipynb` — Python EDA, visualisations and Logistic Regression model

---

## Methods Used
- Exploratory Data Analysis (EDA) with Pandas
- Data visualisation with Matplotlib
- Logistic Regression with Scikit-learn (81.6% accuracy)
- Feature importance analysis
- SQL aggregations, CASE statements, window functions
