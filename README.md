# RavenStack SaaS Churn Analysis

End-to-end churn analysis on a fictional SaaS platform: from exploratory data analysis to ML modeling and business impact quantification.

## Overview
This project investigates churn drivers and revenue impact for RavenStack, a fictional AI-powered collaboration platform. 

The analysis covers:
- Exploratory Data Analysis across 5 relational tables
- Feature engineering and ML modeling (Logistic Regression, Random Forest, XGBoost)
- SHAP-based model interpretability
- Business impact quantification in MRR terms

## Business Question
Which behavioral, product usage, and support signals indicate higher churn risk among SaaS customers, and what is the potential revenue impact?

## Dataset
Synthetic multi-table SaaS dataset from Kaggle by River @ Rivalytics.
- 500 accounts, 5,000 subscriptions, 25,000 feature usage events
- 5 tables: `accounts`, `subscriptions`, `feature_usage`, `support_tickets`, `churn_events`

📎 [Dataset on Kaggle](https://www.kaggle.com/datasets/rivalytics/saas-subscription-and-churn-analytics-dataset)

## Key Findings
- **10.4% of total MRR (\$1.17M/month)** has been lost to churn
- Churned accounts had **higher average MRR** than active ones — RavenStack is losing its most valuable customers
- No single churn driver dominates — churn is multi-causal
- ML models show weak predictive signal, consistent with EDA findings — highlights the importance of data quality in real-world projects

## Business Recommendations
Based on the analysis, RavenStack could reduce churn by:
- Prioritizing retention strategies for high-MRR accounts
- Monitoring feature adoption patterns early in the customer lifecycle
- Investing in data collection to capture stronger behavioral signals

## Tech Stack
Python · Pandas · Scikit-learn · XGBoost · SHAP · Matplotlib · Seaborn

## How to Run
1. Download the dataset from Kaggle (link above)
2. Open the notebook in Google Colab using the button below
3. Update `base_path` in the Setup cell to your own directory
4. Run all cells

## Author
Arianna Galli · [LinkedIn](https://www.linkedin.com/in/arianna-galli)
