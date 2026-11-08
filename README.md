# Datheon Internship Projects

Data analytics projects completed as part of the Datheon internship program, built with Python (Pandas, Matplotlib, Seaborn) in Google Colab.

## Repository Structure
- Superstore_EDA.ipynb : Task 1 notebook
- superstore_sales.csv : Task 1 dataset
- Churn_Analysis.ipynb : Task 3 notebook
- telco_customer_churn.csv : Task 3 dataset

Note: Task 1 notebook reads the file as "Superstore.csv". If you run it, rename superstore_sales.csv to Superstore.csv or update the file name in the first cell.

---

## Task 1: Exploratory Data Analysis on Superstore Retail Sales

**Objective:** Analyze purchase volume, monthly seasonality, category-wise revenue and discount sensitivity.

**Approach:**
1. Loaded the dataset and profiled missing values
2. Removed blank rows and duplicates, parsed order dates and extracted Year-Month
3. Aggregated Sales and Profit by Category, Region, Segment and Sub-Category
4. Visualized monthly sales trends and discount vs profit
5. Documented 6 executive takeaways in the notebook

**Key Findings:**
- Sales peak in November (352,461) and December (325,294); February is the weakest month (59,751)
- Technology is the most profitable category (145,455); Furniture has high sales but a margin of only about 2.5%
- Profit turns negative once discounts exceed 20%
- Tables, Bookcases and Supplies are loss-making sub-categories
- West leads in sales and profit; Central has the weakest margin
- Consumer is the largest segment by sales and profit

**Deliverable:** Superstore_EDA.ipynb (cleaning code, charts and annotated findings)

---

## Task 3: Customer Cohort & Churn Analytics

**Dataset:** IBM Telco Customer Churn (7,043 customers, 7,032 after cleaning)

**Approach:**
1. Cleaned TotalCharges (11 blank rows removed) and created a churn flag
2. Calculated baseline churn rate
3. Built tenure cohorts (0-12, 13-24, 25-48, 49-72 months)
4. Compared churn by contract type, payment method and internet service
5. Identified a high-risk segment and built churn and retention heatmaps

**Key Findings:**
- Baseline churn rate is 26.58%
- Churn falls with tenure: 47.68% (0-12 months) down to 9.51% (49-72 months)
- Month-to-month contracts churn at 42.71%, versus 11.28% (one year) and 2.85% (two year)
- Fiber optic customers without Tech Support churn at 49.37% (2,230 customers)
- Electronic check users churn at 45.29%, versus about 15-17% for automatic payments
- Churned customers have a higher median monthly charge (79.65 vs 64.45)

**Recommendations:**
- Offer onboarding support and loyalty incentives in the first 12 months
- Move month-to-month customers to longer contracts with discounts
- Bundle Tech Support with Fiber optic plans
- Encourage automatic payments over electronic check

**Deliverable:** Churn_Analysis.ipynb (cohort analysis, heatmaps, report and recommendations)

---

## Tools
Python, Pandas, Matplotlib, Seaborn, Google Colab
