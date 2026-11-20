# OTT Customer Churn & Revenue Impact Analysis

**Customer Churn & Retention Analysis using SQL, Python, SQLite, Customer Segmentation and Business KPIs.**

## Project Summary

Analysed OTT subscription churn using SQL and Python by integrating customer, subscription and support data across 3 relational tables. Identified **28.57% overall churn**, quantified **2,047 in lost Customer Lifetime Value (11.84% of total CLTV)**, and uncovered high-churn segments across Basic-plan customers (60%) and Referral-acquired customers (83.33%). Translated analytical findings into actionable recommendations for customer retention and revenue protection.

## Business Overview

Customer churn directly affects recurring revenue, customer lifetime value and long-term business growth in subscription-based businesses.

The objective of this project was to analyse customer churn for an OTT subscription platform, identify high-risk customer segments, evaluate subscription performance, measure customer lifetime value at risk and develop data-backed retention recommendations.

## Business Problems

The analysis focused on answering the following business questions:

- What is the overall customer churn and retention rate?
- Which subscription plans have the highest churn?
- Which customer acquisition channels show higher churn?
- How much Customer Lifetime Value is lost due to churn?
- What is the relationship between customer support activity and churn?
- Which customer segments should be prioritised for retention?

## Dataset & Technology

**Database:** SQLite

The analysis used three relational tables:

| Table | Description |
|---|---|
| `db_customer` | Customer demographics, location and profile information |
| `db_subscription` | Subscription type, plan, contract, monthly charges, CLTV, churn score and cancellation details |
| `db_support` | Complaint dates, support escalations and customer satisfaction scores |

**Dataset Scope:** 21 customer records, with 21 unique customer IDs in customer and subscription data and 7 unique customers in support data.

**Technology Stack:** SQL, SQLite, Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.

## Analysis & Methodology

### 1. Data Extraction & Integration

- Connected Python to SQLite using `sqlite3`.
- Inspected database tables, columns and records.
- Integrated customer, subscription and support data using `customerid`.
- Created a consolidated customer-level dataset containing 21 records and 21 columns.

### 2. Data Cleaning & Preparation

- Standardised customer demographic and categorical values.
- Converted subscription and complaint date columns into datetime format.
- Handled missing country values using state-country mapping.
- Removed unnecessary columns.
- Consolidated support records to one latest record per customer.

### 3. Feature Engineering

- Created a binary churn flag using cancellation dates.
- Calculated customer tenure in days.
- Prepared customer support escalation and complaint indicators.
- Segmented customers into Low, Medium and High churn-risk categories using churn scores.

### 4. Business & KPI Analysis

Calculated and analysed business metrics covering:

- Overall churn and retention rates.
- Churn by subscription plan.
- Churn by acquisition type.
- Revenue at risk from churned customers.
- Average Revenue Per User (ARPU).
- Average customer tenure.
- Total CLTV and CLTV lost due to churn.
- CLTV loss percentage.
- Support escalation rate.
- Average complaints per customer.
- State-level churn patterns.
- Monthly cancellation trends.

### 5. Data Visualisation

Created visualisations using Matplotlib and Seaborn to explore:

- Monthly customer churn trends.
- Churn rate by subscription plan.
- Churn rate by state.
- Relationships between customer and subscription attributes.

## Key Business Results

| Business Metric | Notebook Result |
|---|---:|
| Total Customers | 21 |
| Churned Customers | 6 |
| Overall Churn Rate | 28.57% |
| Retention Rate | 71.43% |
| Basic Plan Churn | 60.00% |
| Standard Plan Churn | 22.22% |
| Premium Plan Churn | 14.29% |
| Organic Acquisition Churn | 0.00% |
| Paid Acquisition Churn | 16.67% |
| Referral Acquisition Churn | 83.33% |
| Average Revenue Per User (ARPU) | 18.85 |
| Average Customer Tenure | 1,586 Days |
| Total CLTV | 17,294 |
| CLTV Lost Due to Churn | 2,047 |
| CLTV Loss Percentage | 11.84% |
| Support Escalation Rate | 19.05% |
| Average Complaints per Customer | 0.33 |
| Revenue at Risk (Notebook Output) | 73.94 |

*Note: Monetary units are not explicitly established in the notebook. Revenue at risk is the sum of monthly charges associated with churned customers, and should not be interpreted as verified MRR without confirming the dataset's revenue definitions.*

## Key Business Insights

### 1. Subscription Plan Performance

The Basic plan recorded the highest churn rate at 60%, compared with 22.22% for Standard and 14.29% for Premium.

**Business implication:** Investigate Basic-plan pricing, service value and customer experience to identify potential reasons for cancellations.

### 2. Customer Acquisition Performance

Referral-acquired customers recorded 83.33% churn, while Paid and Organic acquisition recorded 16.67% and 0% respectively.

**Business implication:** Review the referral customer journey, onboarding process and customer expectations before making acquisition strategy changes.

### 3. Customer Lifetime Value Impact

The analysis calculated total CLTV of 17,294, with 2,047 attributed to churned customers, representing 11.84% of total CLTV.

**Business implication:** Prioritise retention efforts by considering both churn risk and customer lifetime value.

### 4. Customer Retention

The dataset recorded 28.57% churn and 71.43% retention.

**Business implication:** Use customer segmentation and cancellation analysis to identify opportunities for targeted retention campaigns.

### 5. Customer Support Indicators

The support escalation rate was 19.05%, with an average of 0.33 complaints per customer.

**Business implication:** Monitor complaint resolution and escalation patterns as part of customer retention analysis.

## Business Recommendations

1. Investigate the reasons behind higher churn among Basic-plan customers.
2. Review referral acquisition quality and customer onboarding.
3. Prioritise high-risk customers using churn scores and CLTV.
4. Monitor customer complaints, escalations and satisfaction indicators.
5. Develop targeted retention campaigns for vulnerable customer segments.
6. Track churn, retention and CLTV metrics to evaluate retention performance.

## Business Impact

This analysis provides a structured view of customer churn, subscription performance and customer lifetime value exposure.

By identifying high-churn customer segments and quantifying CLTV loss, the analysis supports better prioritisation of retention activities, subscription-plan evaluation and customer experience improvements.

## Project Limitations

- The analysis is based on a small training dataset containing 21 customer records.
- Segment-level churn percentages can change significantly with additional customer records.
- Revenue units and financial definitions require confirmation before interpreting revenue exposure as actual business loss.
- The escalation-versus-churn correlation returned NaN in the notebook and was not used to establish a relationship.
- Findings are exploratory and should be validated using a larger, representative dataset.

## Author

**Mohit Pandey**  
B.Sc. Mathematics | Aspiring Data Analyst

GitHub: https://github.com/MohitPandey-Decode

LinkedIn: https://www.linkedin.com/in/mohit-pandey-data-science
