# Customer Retention Analysis: E-Commerce Churn Drivers

## Executive Summary
This project analyzes a dataset of 1,200 e-commerce customers to understand why users stop using the platform. Using Exploratory Data Analysis (EDA) in Python, the notebook shows that customer complaints and short tenure are the clearest churn risk signals.

The analysis finds a **32.92% churn rate**, and churned customers also show slightly higher average total spend than retained customers, which makes retention especially important.

## Key Business Insights
- Customers who file complaints are much more likely to churn than those who do not.
- Churn risk is highest in the early months of the customer relationship.
- Churned customers have a slightly higher average `TotalSpend`, which suggests the business is losing valuable users.

## Technical Workflow
1. Load and inspect the e-commerce customer dataset.
2. Fill missing values in `Tenure` and `HourSpendOnApp`.
3. Create derived fields such as `TotalSpend` and `Churn_Status`.
4. Explore churn patterns with summary tables and visualizations using Seaborn and Matplotlib.
5. Turn the findings into practical retention recommendations.

## Strategic Recommendations
1. Prioritize complaint resolution for at-risk and high-spending customers.
2. Strengthen onboarding and loyalty efforts during the first 6 months.
3. Build win-back campaigns for churned customers with strong spending history.

## Project Structure
- `churn_analysis.ipynb` - Main notebook with data generation, cleaning, analysis, and charts.
- `ecommerce_customer_data.csv` - Dataset used in the notebook.
- `requirements.txt` - Python dependencies for running the project.

## How To Run
1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Open `churn_analysis.ipynb`.
3. Run all cells from top to bottom to regenerate the tables, charts, and churn summary.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
