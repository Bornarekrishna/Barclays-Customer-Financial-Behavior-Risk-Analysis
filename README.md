# Barclays Customer Financial Behavior & Risk Analysis  
### Barclays Transactional Data – End-to-End Financial Analytics Project

---

## Project Overview

This project analyzes transactional banking data to understand customer financial behavior, liquidity patterns, and potential financial risk exposure.

Using Python-based data analytics techniques, this project performs:

- Data cleaning and transformation  
- Transaction trend analysis  
- Customer segmentation  
- Risk identification  
- Statistical hypothesis testing  

The objective is to derive actionable insights that help financial institutions improve customer engagement, monitor financial risk, and optimize portfolio performance.

---

##  Introduction

With the rapid growth of digital banking transactions, financial institutions must continuously monitor customer behavior, transaction trends, and risk exposure.

This project simulates a real-world financial analytics scenario where customer transactional data is analyzed to:

- Identify spending and deposit patterns  
- Detect dormant or inactive accounts  
- Segment customers by financial activity  
- Detect high-risk financial behavior  
- Validate behavioral assumptions using hypothesis testing  

The dataset spans approximately **18 months (January 2023 – June 2024)** of transactional data.

---

##  Project Objectives

The key objectives of this analysis were:

1. Clean and standardize financial transaction data.
2. Analyze monthly and yearly credit/debit trends.
3. Identify high and low performing accounts.
4. Segment customers based on activity and liquidity.
5. Detect financial risk indicators such as:
   - High withdrawals  
   - Balance volatility  
   - Dormancy  
6. Statistically test whether transaction frequency influences average balance.

---

#  Task 1: Data Cleaning & Formatting

### Actions Performed:

- Removed special characters from financial columns.
- Converted currency fields into numeric format.
- Standardized categorical variables.
- Converted transaction date to datetime format.
- Validated distributions and ensured data consistency.

### Key Insight:

Clean and standardized data ensured accurate aggregation, segmentation, and statistical modeling. The dataset covered 18 months of transactions with balanced categorical distribution.

---

# Task 2: Descriptive Transactional Analysis

### Key Findings:

- Debit transactions (614) significantly exceeded Credit transactions (186).
- All months showed **negative net transaction volume**.
- The highest deficit occurred in **October 2023**.
- 166 accounts were flagged as dormant (≥ 60-day inactivity gap).

### Business Insight:

The portfolio exhibits structurally higher outflows than inflows, indicating spending-dominant behavior. Persistent negative net flow may increase liquidity pressure and overdraft risk.

---

# Task 3: Customer Profile Building

### Activity Segmentation (Quantile-Based Rubric)

- High Activity: 37 accounts  
- Medium Activity: 84 accounts  
- Low Activity: 72 accounts  

### Customer Behavior Segments Identified:

1. **High Net Inflow Accounts**  
   → Financially stable, low-risk customers.

2. **High-Frequency Low-Balance Accounts**  
   → Potential liquidity pressure segment.

3. **Bottom 10% Balance Accounts**  
   → Most financially vulnerable group.

### Insight:

Transaction frequency alone does not determine financial stability. Behavioral segmentation revealed diverse liquidity patterns across the portfolio.

---

# Task 4: Financial Risk Identification

### Risk Indicators Used:

- Large withdrawals (95th percentile threshold)
- Overdraft detection
- Balance volatility (Standard Deviation)
- Z-score anomaly detection

### Observations:

- A small but significant segment shows high balance volatility.
- Persistent negative net flow increases risk exposure.
- High-frequency low-balance customers are most financially vulnerable.

### Risk Insight:

Volatility and transaction behavior should be integrated into internal risk scoring systems for proactive monitoring.

---

# Task 5: Visualization & Exploratory Data Analysis

Visual analysis confirmed:

- Debit dominance across months.
- No month showed positive net inflow.
- Distinct customer behavior clusters exist.
- Long right-tail volatility distribution suggests concentrated risk.

Charts included:

- Monthly Credit vs Debit Trend
- Monthly Net Transaction Volume
- Transaction Type Distribution
- Activity Level Distribution
- Balance Volatility Histogram
- Transaction Frequency vs Average Balance Scatter Plot

---

# Task 6: Hypothesis Testing

### Hypothesis:

Do high-volume accounts maintain significantly higher average balances than low-volume accounts?

### Statistical Results:

- T-statistic: -0.86  
- P-value: 0.392  

Since the p-value > 0.05, we **fail to reject the null hypothesis**.

### Conclusion:

There is no statistically significant difference between high-volume and low-volume accounts in terms of average balance.

### Business Meaning:

Transaction frequency alone is not a reliable predictor of liquidity strength. Risk modeling should incorporate additional behavioral and volatility metrics.

---

# Key Strategic Insights

1. The portfolio is expenditure-heavy.
2. Persistent negative net flow indicates liquidity pressure.
3. A small segment contributes majority positive inflows.
4. High-frequency low-balance accounts represent hidden risk.
5. Risk assessment should include volatility and anomaly detection metrics.

---

# Recommendations for the Bank

### 1️. Proactive Liquidity Monitoring
Implement automated alerts for:
- Consecutive negative net flow months  
- High volatility accounts  
- Frequent large withdrawals  

### 2️. Customer Segmentation-Based Engagement
- Offer investment products to high net inflow customers.
- Provide budgeting tools to high-frequency low-balance customers.
- Re-engage dormant accounts via targeted campaigns.

### 3️. Enhanced Risk Scoring Model
Integrate:
- Balance volatility
- Net inflow trends
- Dormancy indicators
- Transaction anomaly scores

### 4️. Seasonal Monitoring
Increase monitoring during historically high debit months (e.g., October–November).

---

# Tools & Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- SciPy (Statistical Testing)  

---
