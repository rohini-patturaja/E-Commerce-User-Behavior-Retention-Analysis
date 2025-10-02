# 🛍️ E-Commerce User Behavior & Retention Analysis

This project analyzes customer behavior from an e-commerce store using techniques like **A/B testing**, **segmentation**, and **cohort analysis**. It uncovers data-driven insights to improve **user retention**, **monetization**, and overall **business performance**.

---

## 📁 1. Introduction

- **Dataset**: Online Retail data from a UK-based store *(Dec 2010 – Dec 2011)*
- **Objective**: Understand customer value, improve revenue, and test strategic hypotheses
- **Tools Used**:  
  `Python` (Pandas, Matplotlib, Seaborn)  
  `StatsModels`, `Scipy`
- **Core Techniques**:  
  - RFM Segmentation  
  - A/B Testing  
  - Multivariate Testing  
  - Cohort Analysis  

---

## 📊 2. Data Description

- ~500,000 transactions
- Key Fields: `InvoiceDate`, `CustomerID`, `Quantity`, `UnitPrice`, `Country`, `Description`
- Filtered to include:
  - Only **UK customers**
  - Only **non-cancelled transactions**
- New Field Created:
  - **Revenue = Quantity × UnitPrice**

---

## 🎯 3. Business Impact

- Identify **high-value users** and segments
- Simulate **pricing/discount** strategies
- Analyze **long-term customer behavior**
- Build **actionable insights** for marketing and product teams

---

## 🧩 4. Segmentation – RFM Analysis

> **RFM = Recency, Frequency, Monetary**

- Customers grouped into RFM scores (e.g., **444** = best)
- 📌 **Key Findings**:
  - 460 customers were in top **RFM 444** segment
  - Average revenue of **RFM 444s**: £7,948
  - These users are **repeat buyers** with high lifetime value

---

## 🧪 5. A/B Testing – Discount Simulation

- Simulated 50/50 split:
  - **Test Group**: Received 10% discount
  - **Control Group**: No discount
- **Metrics Compared**:
  - Conversion Rate
  - ARPU (Average Revenue per User)

📉 **Result**:
- Control group outperformed test group
- No statistically significant improvement in ARPU *(p = 0.33)*
- **Flat discounting is not effective**

---

## 🧪 6. Multivariate Testing – Discount × Category

- Tested combinations of:
  - `discount_flag` (yes/no)
  - `product category` (Clothing, Home, Toys, Other)

📌 **Key Insights**:
- Discount alone: Not significant *(p = 0.37)*
- No interaction between discount and category
- **Product category** had marginal significance *(p ≈ 0.05)*
- ➤ Focus on **category-specific strategies** instead of generic promotions

---

## 📆 7. Cohort Analysis – Retention

- Grouped users by **first purchase month**
- Tracked **monthly retention** for 12 months

📈 **Insights**:
- **December 2010** cohort had highest long-term retention  
  → 50% still active in **Month 11**
- Most cohorts dropped to **20–30% by Month 3**
- Feb–Apr 2011 cohorts showed moderate improvement

---

## 💰 8. Cohort Analysis – Revenue

### 🔹 Total Revenue by Cohort
- **December 2010** generated the highest revenue across all months
- March & May cohorts had revenue spikes in later months

### 🔹 Average Revenue per User (ARPU)
- **Normalized** to remove cohort size bias
- **August 2011** peaked at **£1,218 per user** in Month 3
- **May 2011**, Month 7 had outlier revenue: **£7,696 per user**
- Helped identify **quality over quantity** in customer behavior

---

## ✅ 9. Summary

This project walks through the **complete customer analytics lifecycle** using real-world e-commerce data.

### 🔍 Exploratory Data Analysis (EDA)
- Identified trends in **daily revenue**, **top products**, and **geographic patterns**

### 📊 RFM Segmentation
- Grouped users by Recency, Frequency, and Monetary scores  
- **Top segment (444)** had high engagement and LTV  
→ Ideal for loyalty or premium offers

### 🧪 A/B Testing
- Tested blanket discounts  
- No uplift in conversion or revenue  
→ Blanket discounts not effective

### 🧪 Multivariate Testing
- Found product category affects purchase more than discounts  
→ Use **category-targeted offers** instead

### 📆 Cohort Retention
- December 2010 cohort retained **50% of users** by Month 11  
→ Successful acquisition or seasonality

### 💰 Cohort Revenue
- Normalized revenue showed **hidden value** in smaller cohorts  
→ Focus on ARPU, not just total revenue

---

## 💡 10. Business Recommendations

- ✅ Prioritize **RFM 444** customers for loyalty and upsell programs
- 🚫 Avoid **flat discounts** – they don’t drive revenue growth
- 🎯 Segment by **product category** for promotional targeting
- 📈 Improve **onboarding flows** for cohorts with early drop-off
- 🔁 Use **cohort analysis monthly** to track retention and LTV

---

## 📌 Tools & Technologies

| Category           | Tools Used                                  |
|--------------------|----------------------------------------------|
| **Programming**    | Python                                       |
| **Libraries**      | Pandas, Matplotlib, Seaborn, StatsModels     |
| **Analysis**       | A/B Testing, Multivariate Testing, RFM, Cohorts |
| **Data Source**    | Online Retail CSV (UK-based e-commerce)      |

---


