📚 E-Commerce Sales Analysis

📝 Project Overview

This project analyzes sales and customer behavior for an e-library using three datasets. The goal is to extract key insights, visualize revenue trends, and apply statistical tests to understand purchasing behaviors.

📂 Datasets
```text
We used three CSV files:

transactions.csv (687,535 rows, 4 columns)

id_prod (Product ID)
date (Transaction Date)
session_id (Session Identifier)
client_id (Customer ID)
products.csv (3,287 rows, 3 columns)

id_prod (Product ID)
price (Product Price)
categ (Product Category)
customers.csv (8,622 rows, 3 columns)

client_id (Customer ID)
sex (Gender)
birth (Birth Year)

🔍 Key Steps & Analysis
✔️ Data Preparation

Clean datasets were provided; minor transformations applied.
Merged tables using id_prod and client_id with a datetime feature (year-month-day).

✔️ Exploratory Data Analysis (EDA)

Demographic insights: Age distribution, gender proportions.
Product performance: Bestsellers vs. low-performing products.
Revenue analysis:
Evolution of total revenue over time.
Top and bottom-selling products by category.
Lorenz curve & Gini index to assess revenue concentration.

✔️ Statistical Tests

Chi-square test: Association between two categorical variables.
Pearson correlation: Relationship between two numerical variables.
ANOVA alternative:
Normality & variance tests (Kolmogorov-Smirnov, Levene) showed ANOVA was not applicable.
Used Kruskal-Wallis test (non-parametric ANOVA alternative).

🛠️ Tools & Technologies
Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Statsmodels)
Jupyter Notebook

📈 Results & Insights
Sales revenue fluctuates across months, with clear seasonality.
Certain product categories drive a disproportionate share of revenue (high Gini index).
No significant correlation between gender and spending habits.
Alternative statistical tests confirmed variations in purchasing behavior across customer segments.

📌 Next Steps
Implement clustering for customer segmentation.
Explore predictive models for sales forecasting.
Further investigate price elasticity and discount impacts.

📎 Repository Structure
/ecommerce-analysis  
│── data/            # Raw & processed datasets  
│── notebook/       # Jupyter notebooks with analysis   
│── README.md        # Project documentation  
💡 Feel free to suggest improvements or contribute! 🚀
