# Customer Retention Analysis: E-Commerce Churn Drivers

## Executive Summary
This project analyzes a dataset of 1,200 e-commerce customers to understand why users stop using the platform. By performing Exploratory Data Analysis (EDA) in Python, I identified that **customer complaints** and **early-stage tenure (0-6 months)** are the most significant predictors of churn. 

The analysis reveals a **32.92% churn rate**, with high-value spenders being at a surprisingly high risk of leaving.

---

## Key Business Insights
* **The "Complaint" Red Flag:** Customers who log a complaint are **3x more likely** to churn. Our current "save" rate for frustrated customers is critically low.
* **The Vulnerability Window:** Churn is most aggressive in the first **5 months**. If a customer reaches the 8-month mark, their likelihood of staying increases by 40%.
* **High-Value Attrition:** Churned customers actually had a higher `TotalSpend` ($301) than retained customers ($295), meaning we are losing our most profitable users.

---

## Technical Workflow
1.  **Data Cleaning:** Handled missing values in `Tenure` and `AppUsage` using median imputation to maintain data integrity.
2.  **Feature Engineering:** Calculated `TotalSpend` and created categorical bins for churn status to simplify visualization.
3.  **Exploratory Analysis:** Utilized **Seaborn** and **Matplotlib** to create correlation plots, boxplots for tenure distribution, and countplots for behavioral analysis.
4.  **Statistical Summaries:** Grouped data by churn status to create "Customer Profiles" for the marketing department.

---

## Strategic Recommendations
1.  **Prioritize Complaint Resolution:** Implement an automated "High Priority" flag for tickets from customers with a `TotalSpend` above $250.
2.  **Onboarding Loyalty Program:** Launch a "6-Month Milestone" reward to bridge the gap between new users and long-term loyalists.
3.  **Win-Back Campaigns:** Target churned high-spenders with personalized incentives, as they have already demonstrated high lifetime value.

---

## Project Structure
* `churn_analysis.ipynb`: The complete Python notebook containing code and visualizations.
* `ecommerce_customer_data.csv`: The raw dataset used for the analysis.
