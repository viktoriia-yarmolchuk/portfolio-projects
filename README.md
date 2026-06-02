# Data Analytics Portfolio Projects

Welcome! This repository contains my data analytics portfolio projects. These practical cases demonstrate my ability to extract, process, and analyze data to find business insights and test statistical hypotheses.

## Projects in this Repository

### 1. [Analysis of A/B Testing Results](https://github.com/viktoriia-yarmolchuk/portfolio-projects/blob/main/analysis_of_ab_testing_results.ipynb)
**Description:**
This project analyzes A/B test data using an automated Python script connected to a Google BigQuery dataset. The goal is to evaluate the statistical significance of changes across different user segments and metrics.

**Key Steps and Tasks:**
- **Data Extraction:** Queried and aggregated session, event, and order data directly from Google BigQuery using SQL.
- **Automated Statistical Analysis:** Developed an Object-Oriented `ABTestAnalyzer` Python class to calculate conversions and automatically perform a two-sample z-test for proportions using the `statsmodels` library.
- **Metric Tracking:** Evaluated the performance of specific metrics such as `add_shipping_info/session`, `begin_checkout/session`, and `new_accounts/session` against a standard significance level ($\alpha=0.05$).
- **Data Visualization:** Built a Tableau dashboard to visualize traffic split validation, conversion rates, and the statistical significance of results across various channels, devices, and countries.

**Tech Stack:** `Python` (`Pandas`, `Numpy`, `Statsmodels`), `SQL` (Google BigQuery), `Tableau`.

---

### 2. [E-commerce Sales Analysis](https://github.com/viktoriia-yarmolchuk/portfolio-projects/blob/main/analysis_of_ecommerce_sales.ipynb)
**Description:**
An exploratory and statistical analysis of over 349,000 e-commerce user sessions and transaction records spanning from November 2020 to January 2021. The objective is to identify key revenue drivers, assess purchasing behavior, and validate business trends.

**Key Steps and Tasks:**
- **Data Processing:** Joined multiple tables (sessions, orders, products, accounts) using BigQuery SQL and handled missing values that naturally occurred during the data integration process.
- **Business Metrics Calculation:** Calculated core Key Performance Indicators, identifying a Total Revenue of $31.97 million, an Average Order Value (AOV) of $953.3, and a Conversion Rate of 9.59%.
- **Exploratory Data Analysis (EDA):** Analyzed sales dynamics and segmented performance by geography (with the US leading), product category (highlighting Sofas & armchairs), device type, and traffic channel (Organic Search).
- **Statistical Testing:** Utilized the D'Agostino-Pearson test for normality and Spearman's rank correlation coefficient (0.865) to confirm a statistically significant positive relationship between session volume and total sales.
- **Strategic Recommendations:** Formulated actionable business advice regarding assortment optimization for top-performing categories and geographic marketing expansion into promising regions like India and Canada.

**Tech Stack:** `Python` (`Pandas`, `Matplotlib`, `Seaborn`, `SciPy`), `SQL` (Google BigQuery), `Tableau`.

---

### 3. [Global Retail Sales & Profitability Analysis](https://github.com/viktoriia-yarmolchuk/portfolio-projects/blob/main/global_retail_sales_analysis.ipynb)
**Description:**
This project focuses on a comprehensive Exploratory Data Analysis (EDA) of global retail transactions across 45 countries spanning from 2010 to 2017. The primary objective is to evaluate product profitability, assess regional market performance, compare offline and online sales channels, and analyze supply chain efficiency through order delivery times.

**Key Steps and Tasks:**
- **Data Cleaning & Feature Engineering:** Merged multiple datasets (sales events, products, countries), handled missing values and anomalous country codes (e.g., Namibia 'NA'), corrected data types, and calculated new metrics such as profit and delivery time.
- **Profitability Analysis:** Evaluated revenue and profit by product category, identifying Cosmetics as the most profitable segment (over $92.7 million) despite Office Supplies and Beverages leading in total units sold.
- **Geographic & Channel Performance:** Mapped profit distribution across global regions, pinpointing Europe (specifically Southern Europe) as the dominant market contributing 94.7% of total profit, and compared the relatively even split between Offline (50.6%) and Online (49.4%) sales channels.
- **Logistics Evaluation:** Analyzed order fulfillment efficiency by calculating average and median delivery times across product types and regions, and statistically verified that there is no direct correlation between delivery speed and final profit.
- **Trend Dynamics:** Investigated year-over-year sales and profit trajectories, highlighting significant shifts in consumer demand, such as a 125% growth in the Vegetables category compared to a 50% decline in Cereal sales between 2010 and 2016.

**Tech Stack:** `Python` (`Pandas`, `NumPy`, `Matplotlib`, `Seaborn`).
