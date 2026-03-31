# E-Commerce User Behavior & Retention Analysis
Decoding 500,000 Transactions to Understand Who Your Best Customers Are — and How to Keep Them

Most businesses know their revenue. Very few know which customers are quietly generating most of it, and which ones are one bad experience away from leaving forever. This project closes that gap.

---

## The Business Problem

Running an e-commerce store without behavioral analytics is like navigating a city without a map. This project analyzes over 500,000 UK-based transactions to answer critical business questions:

- Who are the highest-value customers?
- Do discounts actually increase revenue?
- Are customers being retained or lost after first purchase?
- Which cohorts drive long-term value?

---

## Dataset Overview

| Attribute            | Detail                          |
|---------------------|--------------------------------|
| Total Transactions  | ~500,000 records               |
| Time Period         | Dec 2010 – Dec 2011            |
| Geography           | UK only                        |
| Key Fields          | Invoice Date, Customer ID, Quantity, Unit Price |
| Engineered Feature  | Revenue = Quantity × Unit Price |
| Scope Filter        | Non-cancelled transactions     |

---

## Tech Stack

- **Data Processing:** Python, Pandas  
- **Visualization:** Matplotlib, Seaborn  
- **Statistical Testing:** StatsModels, SciPy  
- **Core Methods:** RFM Segmentation, A/B Testing, Multivariate Testing, Cohort Analysis  

---

## Data Cleaning & Preparation

- Removed cancelled transactions and duplicates  
- Filtered to UK-only customers for consistency  
- Engineered revenue feature  
- Created RFM (Recency, Frequency, Monetary) metrics  

---

## Methodology

### 1. RFM Segmentation
Identified high-value customers based on purchase behavior.

- Top segment (RFM 444): 460 customers  
- Average revenue per customer: £7,948  
- Represents the most loyal and profitable users  

---

### 2. A/B Testing (Discount Impact)

- Simulated 10% discount vs no discount  
- Control group outperformed test group in ARPU  
- Result: No statistically significant uplift (p = 0.33)  

Conclusion: Blanket discounts reduce margin without increasing revenue.

---

### 3. Multivariate Testing

- Tested interaction between discount and product category  
- Discount effect remained insignificant (p = 0.37)  
- Product category showed stronger influence on purchase behavior  

Conclusion: Product relevance matters more than pricing incentives.

---

### 4. Cohort Analysis

Measured retention across customer cohorts.

- December 2010 cohort: 50% retention at Month 11  
- Typical cohorts: drop to 20–30% by Month 3  
- August 2011 cohort: high ARPU despite small size  

Conclusion: Customer quality varies significantly by acquisition timing.

---

## Key Findings

- High-value customers (RFM 444) drive disproportionate revenue  
- Discounts do not significantly improve performance  
- Product category influences behavior more than promotions  
- Retention drops sharply within first 3 months  
- Small, high-value cohorts outperform large low-value cohorts  

---

## Recommendations

1. Focus on retaining high-value RFM segments  
2. Eliminate blanket discount strategies  
3. Invest in category-based targeting  
4. Analyze and replicate high-retention cohorts (Dec 2010)  
5. Introduce retention interventions before Month 3 drop-off  
6. Measure acquisition quality using ARPU, not just volume  
7. Track cohort performance on a recurring basis  

---

## Conclusion

This project demonstrates that sustainable growth comes from understanding customer behavior at a granular level. Aggregate metrics hide critical insights, while segmentation, experimentation, and cohort analysis reveal the true drivers of revenue and retention.

The findings challenge common assumptions:
- Discounts are not always effective  
- Customer quality matters more than volume  
- Retention patterns define long-term success  

Businesses that leverage these insights can move from reactive decision-making to data-driven strategy.

---

## Tools & Data

- Python, Pandas, Matplotlib, Seaborn  
- StatsModels, SciPy  
- Dataset: UCI Online Retail (UK-based transactions)

---

## Author

Rohini Patturaja  
© 2025
