# Bank Customer Churn Analysis

## Overview
This project analyses a dataset of 10,000 bank customers to identify why customers churn and predict which customers are likely to leave. Using SQL, I uncovered key churn patterns, visualised findings with Python, and built a Logistic Regression model that predicts customer churn with 81.6% accuracy.

**Tools used:** SQL (SQLite) · Python · Pandas · Matplotlib · Scikit-learn

## Key Findings
-  **Germany** churns at 32% — double the rate of France and Spain (16%)
-  Customers with **4 products** have a **100% churn rate** — the bank is overselling
-  Customers aged **46-60** are the highest risk group at **51% churn**
-  **Logistic Regression model** achieves **81.6% accuracy** predicting churn

## Project Structure
- `churn_analysis.sql` — SQL queries analysing churn patterns
- `Bank_Customer_Churn_Analysis.ipynb` — Python EDA, visualisations and ML model

## Business Recommendations
1. Investigate why German customers churn at double the rate — pricing or product fit issue
2. Cap product cross-selling at 2 products per customer — beyond this, churn increases sharply
3. Create targeted retention campaigns for the 46-60 age segment
