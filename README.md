# E-commerce Funnel & Revenue Analysis

## Objective
To analyze user behavior across funnel stages and calculate key revenue metrics using SQL in BigQuery.

---

## Dataset
Dataset contains user events with the following fields:
- user_id
- event_id
- event_type  
- event_date  
- amount
- product_id
- traffic_source

Data is stored in BigQuery.

---

## Analysis Performed
- Funnel stage analysis (page_view → purchase)  
- Revenue analysis (total revenue, AOV, revenue per user)  
- Date-based filtering for monthly analysis  

---

## Insights & Recommendations

### 1. UX & Website Optimization
**Don't Touch the Checkout Flow:**  
The conversion rates from Checkout Start → Purchase are excellent (~85%+). This indicates the technical payment flow is frictionless.  

**Action:**  
Do not redesign the checkout page right now; you risk breaking something that is working perfectly.

---

### 2. Marketing Strategy
**Stop Over-Investing in Social for Sales:**  
Social Media is driving 30% of our traffic (Volume) but has the lowest conversion rate (Efficiency). We are likely paying for "window shoppers."  

**Action:**  
Shift budget away from "Traffic" objectives on social ads and focus on "Retargeting" or "Lead Gen" to capture emails instead.  

**Double Down on Email Marketing:**  
Email is our highest converting channel (~35%+ email conversion rate vs ~5% for Social).  

**Action:**  
Implement an aggressive email capture popup for those high-volume Social visitors. If we can get them onto our email list, our data proves they are far more likely to buy later.

---

### 3. Financial & Revenue
**Audit Ad Spend against AOV:**  
We found our Average Order Value is ~$95.  

**Action:**  
Set a strict Customer Acquisition Cost (CAC) limit. If we are paying more than $20–$30 to acquire a customer via Social Media ads (which convert poorly), we are likely losing money on those specific transactions.
