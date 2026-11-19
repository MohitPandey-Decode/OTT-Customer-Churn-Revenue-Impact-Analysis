# OTT-Customer-Churn-Revenue-Impact-Analysis
OTT Customer Churn &amp; Retention Analysis using SQL, Python, 20+ KPIs, Customer Segmentation and Business Insights.


## Business Overview
Customer churn is a major challenge for subscription-based businesses. When customers cancel their subscriptions, businesses lose recurring revenue and potential customer lifetime value (CLTV).

The objective of this project was to analyze customer churn for an OTT subscription business, identify high-risk customer segments, understand subscription cancellation patterns, and recommend strategies to improve customer retention and protect recurring revenue.

## Business Problem
The business wanted to understand:

- Which customers are churning?
- Which subscription plans have the highest churn?
- Do monthly or annual subscribers have higher churn?
- How do customer support escalations relate to churn?
- How much recurring revenue and customer lifetime value are at risk?
- What actions can improve customer retention?

## Data & Technology
**Database:** Customer Churn (SQLite)

Three relational tables were analyzed:

1. `db_customer` – Customer demographics, country, state and profile information.
2. `db_subscription` – Subscription type, plan, contract, monthly charges, cancellation details, CLTV and churn score.
3. `db_support` – Complaint dates, escalations and customer satisfaction scores.

**Technology Stack:** SQL, SQLite, Python, Pandas, NumPy, Matplotlib, Seaborn.

## What I Did

### 1. Data Extraction & Integration
- Connected Python with SQLite using `sqlite3`.
- Extracted data from three relational tables.
- Integrated customer, subscription and support information using `customerid`.

### 2. Data Cleaning & Preparation
- Standardized customer information and categorical values.
- Converted date columns into appropriate datetime formats.
- Handled missing country values using state-country mapping.
- Removed unnecessary columns and prepared data for analysis.

### 3. Feature Engineering
- Created a churn flag using cancellation dates.
- Calculated customer tenure and churn-related indicators.
- Prepared customer support and escalation features.
- Segmented customers using churn-score risk categories.

### 4. Business Analysis
Analyzed 20+ business KPIs across customer churn, retention, subscription plans, contract types, revenue, customer lifetime value and support interactions.

Key techniques included:
- SQL and SQLite data extraction
- Pandas aggregation and group-by analysis
- Pivot tables
- Customer segmentation
- Correlation analysis
- Exploratory data analysis
- Data visualization

## Key Business Results

| Business Metric | Result |
|---|---:|
| Overall Churn Rate | 28.6% |
| Retention Rate | 71.4% |
| Monthly Contract Churn | 55.6% |
| Annual Contract Churn | 8.3% |
| Basic Plan Churn | 60.0% |
| Standard Plan Churn | 22.2% |
| Premium Plan Churn | 14.3% |
| Average Customer Tenure | 1,451 Days |
| ARPU | Rs 18.8 |
| Total Revenue | 395 |
| Revenue Loss Due to Churn | 74 |
| CLTV Lost | 2,047 |
| Revenue Loss Percentage | 18% |

The trainer's quantified portfolio summary additionally reports:
- $73.94 per month in MRR leakage.
- $2,047 in CLTV erosion attributed to six at-risk customers.

## Business Insights

**1. Contract Type & Churn**

Monthly subscribers recorded 55.6% churn compared with 8.3% for annual subscribers. This indicates a significant retention gap between contract segments.

**2. Subscription Plan Performance**

The Basic plan had the highest churn rate at 60%, while Premium had the lowest at 14.3%.

**3. Revenue Impact**

The reference analysis reported 74 in revenue loss due to churn, an 18% revenue loss rate, and 2,047 in CLTV lost.

**4. Geographic & Time-Based Trends**

September 2024 was identified as the highest-churn month, while Karnataka was identified as the most affected state.

**5. Customer Support & Risk**

Support escalations, CSAT scores and churn-risk segments were considered important dimensions for identifying customers who may require retention attention.

## Business Recommendations

1. Prioritize monthly subscribers for targeted retention campaigns.
2. Investigate Basic plan pricing, benefits and customer experience.
3. Prioritize medium- and high-risk customers using churn scores and customer lifetime value.
4. Investigate customer complaints, escalations and low CSAT scores.
5. Review cancellation reasons, including competitor switching and pricing sensitivity.
6. Evaluate annual subscription incentives and contract-migration strategies.
7. Monitor retention rate, recurring revenue and CLTV to measure the impact of retention initiatives.

## Business Impact

The analysis identifies customer segments with higher churn exposure and quantifies potential recurring-revenue and lifetime-value losses.

These findings provide a data-backed basis for prioritizing retention campaigns, reviewing subscription strategies and improving customer experience.

## Project Limitations

This is a portfolio analysis based on a training dataset. The customer/subscription dataset contains 21 records. Reported metrics are dataset estimates and should not be interpreted as audited company financial results or guaranteed profit improvements.

## Author
**Mohit Pandey**  
B.Sc. Mathematics | Aspiring Data Analyst

GitHub: https://github.com/MohitPandey-Decode  
LinkedIn: https://www.linkedin.com/in/mohit-pandey-data-science
