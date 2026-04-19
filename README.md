# Tunia Technologies – Sales & Performance Dashboard
> End-to-end data pipeline, multi-dimensional analysis, and interactive dashboard built entirely in Microsoft Excel.

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-ETL_Pipeline-217346?style=for-the-badge)
![Pivot tables](https://img.shields.io/badge/Pivot-table-217346?style=for-the-badge)
![ Dashboard](https://img.shields.io/badge/Dashboard-visualization-CF222E?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)


Tunia Technologies is a Pan-African tech-driven company founded in 2019, operating across three core verticals: Marketplace, Logistics, and Payment Services. The company has grown steadily across multiple regions in Africa and is now seeking deeper insight into its operational performance using historical sales data.


**A comprehensive data analytics project transforming 2022 transactional data into actionable business intelligence.**

---

## Table of Contents

- [Executive Summary](#executive-summary)
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Project Objectives](#project-objectives)
- [Process Flow & Methodology](#process-flow--methodology)
- [Key Insights](#key-insights)
- [Business Impact](#business-impact)
- [Recommendations](#recommendations)


---

## Executive Summary

[Click here to view the Executive Summary PDF](./Executive%20summary%20for%20Tunia.pdf)

Tunia Technologies generated $2.30M in revenue and $286.4K in profit, resulting in a ~12.5% margin. While revenue performance is strong, profitability is constrained by product losses and inconsistent discounting.

Sales improved significantly during the year, rising from $59.8K in February to $352.5K in November (~489% growth), with December maintaining strong performance at $323.5K. However, this growth is heavily concentrated in the final months.

The Technology category contributes $836.2K (~36%) of total revenue, making it the primary growth driver. While this category is a strong growth driver with high margins, the level of dependence introduces risk if performance weakens.

Profit is led by the Consumer segment at $134.1K, outperforming Corporate ($91.98K) and Home Office ($60.30K) by ~46% and ~122% respectively, indicating stronger pricing and demand in the consumer market.

At the same time, a group of underperforming products: including printers and conference tables- generates over $17+K in losses, directly impacting overall profitability. At the same time, inconsistent discounting, such as $567 applied to Binders versus ~$100–$137(papers, chairs, furnishings, phone) across other categories, suggests weak pricing discipline.

The business shows strong demand and growth potential but requires better control over costs, pricing, discounting,  and product performance to improve profitability.

This analysis identifies **5 high-impact strategic opportunities** that can improve profit retention and reduce operational risk, with projected gains of **$150K–$250K in additional annual profit**.


---

## Project Overview

**Client:** Tunia Technologies – A Pan-African tech-driven company founded in 2019  
**Industry Verticals:** Marketplace, Logistics, Payment Services  
**Project Scope:** Sales and operational performance analysis using 2022 transactional data  
**Data Period:** January – December 2022

Tunia Technologies operates across multiple African regions with diverse customer segments (Consumer, Corporate, Home Office) and product categories (Technology, Furniture, Office Supplies). Despite rapid growth, the business faced **visibility gaps** into which products, segments, and categories were truly driving profit; not just revenue.

**Dataset Composition:**

1. **9,994 sales transactions**
   
2. **37,873 units sold**
   
3. **Key dimensions:** Order Date, Ship Date, Ship Mode, Customer Segment, Region, Category, Sub-Category, Product, Sales, Profit, Quantity, Discount

---

## Problem Statement

Tunia Technologies demonstrated **strong sales growth** across 2022, but profit growth did not scale proportionally. Three critical challenges emerged:

### **1. Profit Margin Erosion**
Despite $2.30M in revenue, profit margin remained low at **12.5%**, indicating:

1. Heavy discounting without clear performance justification
   
2. Loss-making product SKUs are not being addressed

### **2. Revenue Concentration & Demand Imbalance**
Sales peaked at **$352.5K in November** but averaged only **$159.8K in non-Q4 months**, creating:

1. Over-reliance on year-end demand (Q4 concentrated **~42% of annual sales**)
   
2. Increased operational risk if seasonal demand shifts
 
3. Inefficient workforce and inventory planning across low-demand months

### **3. Lack of Segment & Product-Level Performance Visibility**
Leadership could not distinguish between high-profit and low-profit drivers:

1. Some products generated **losses exceeding -$17k+** (e.g., Cubify printers)
 
2. Discount allocation was inconsistent ($567 on Binders vs. ~$100–$137 elsewhere)

3. Segment profitability varied by **122% between best and worst performers**, but root causes were unclear

---

## Project Objectives

This analysis was designed to achieve **four core objectives:**

1. **Identify Revenue & Profit Drivers**

2. **Expose Margin Leakage Points**

3. **Enable Data-Driven Decision Making**
   - Create interactive visualizations that allow filtering by Ship Mode, Region, and Time Period
    
4. **Support Strategic Planning**


---
## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | End-End Analysis |
| **Power Query** | ETL / Data Transformation |
| **Pivot Tables** | Multi-dimensional Analysis |
| **Pivot Charts & Slicers** | Interactive Dashboarding |
| **Advanced Formulas** | KPI & Metric Calculations |
## Process Flow & Methodology

## 1. Data Extraction

Extracted 2022 transactional data from Tunia Technologies' operational system and identified **three data quality issues** requiring remediation before analysis could begin.

**Issues identified:**

1. Missing values in the discount and shipping mode fields
   
2. Inconsistent date formatting (mixed `MM/DD/YYYY` and `DD/MM/YYYY`)
  
3.  Duplicate order records

---

## 2. Data Cleaning & Transformation

**Transformation steps applied:**

1. Standardized all date formats to `YYYY-MM-DD`
 
2. Removed duplicate records based on Order ID, Customer Name, and Order Date
 
3. Validated data integrity — confirmed **9,994 unique transactions** post-cleaning

4. Created derived fields for downstream analysis:

| Derived Field | Formula / Logic |
|---|---|
| **Profit Margin %** | `(Profit / Sales) × 100` |
| **Month & Quarter** | Extracted from Order Date |
| **Discount Rate %** | `(Discount / Sales) × 100` |

---

## 3. Data Modelling & Analysis

Structured data by key dimensions to enable multi-level aggregation across the business.

**Hierarchical Dimensions:**

| Dimension | Levels |
|---|---|
| **Product** | Product → Sub-Category → Category |
| **Customer Segment** | Consumer, Corporate, Home Office |
| **Ship Mode** | First Class, Same Day, Second Class, Standard |
| **Time** | Month → Quarter → Year |
| **Region** | Geographic territories |

### **4 Visualization & Dashboard Development**
Visualization & Dashboard Development
Built an interactive Excel dashboard surfacing performance across sales, profit, discounting, and logistics.

Tools Used: Microsoft Excel (Pivot Tables, Pivot Charts, Slicers, Conditional Formatting)

 KPI Summary
Five headline metrics pinned at the top of the dashboard for at-a-glance performance monitoring:

1. Count of Sales : Total number of transactions processed in 2022

2. Sum of Sales : Total revenue generated across all orders
 
3. Sum of Profit : Overall profit contribution across the business
   
4. Sum of Discount : Aggregate discount value applied across transactions
   
5. Sum of Quantity : Total units sold across all product lines


 Trend Analysis

Monthly Sales Trend (line chart): Tracks revenue movement across all 12 months of 2022, surfacing demand seasonality, peak trading periods, and slowdown windows


 Category & Segment Performance

Sales by Category (donut chart): Visualizes revenue share across product categories, identifying where demand is concentrated and where growth gaps exist

Profit by Segment (pie chart):  Breaks down profit contribution by Customer Segment (Consumer, Corporate, Home Office), isolating the most and least profitable customer bases


 Risk Visualization

Top 5 Most Discounted Sub-Categories: Highlights the sub-categories carrying the highest discount burden, flagging potential margin erosion risk

Bottom 5 Loss-Making Products: Surfaces' individual products generating negative profit, enabling targeted review for pricing, discontinuation, or cost restructuring


 Dynamic Filtering

Ship Mode Slicer (First Class, Same Day, Second Class, Standard) — Enables real-time filtering of all dashboard visuals by logistics mode, allowing isolated performance analysis per shipping channel

---

## Key Insights

### **1. Revenue Growth is Strong, but Profit Retention is Limited**

**Finding:** Despite strong sales, the 12.5% profit margin indicates significant value leakage. In healthy tech/commerce operations, margins typically range **18–25%**. This gap is driven by two factors:

i. **Excessive discounting:** $1,561 in total discounts, with inconsistent application across products

ii. **Product losses:** Loss-making Stock Keeping Unit(SKUs) contribute **-$17K+ in combined losses**


---

### **2. Sales Growth is Heavily Skewed Toward Year-End**

**Finding:** Sales exhibit extreme seasonality, with Q4 (October–December) accounting for **42% of annual revenue**. November alone drives **$352.5K (15.3% of total)**, while February bottoms out at $59.8K. This **5.9x monthly variance** indicates:

i. Strong holiday/year-end demand pull

ii. Weak early-year customer engagement

iii.Risk concentration: If Q4 demand drops 10–15%, annual profit could decline by **$30–40K*

---

### **3. Technology Category Drives the Largest Share of Revenue and Operates at High Margins**

**Finding:** Technology ($836,154) is the dominant revenue driver and operates at significantly higher margins than other categories. This category combines:

i. **High demand:** 36.4% of all sales

ii. **Strong margins:** Estimated ~31.8% profit margin (compared to 10–13% for Furniture($742k) and 3–4% for Office Supplies($719k))

iii. **Scalability:** Room to increase inventory and marketing allocation

However, **heavy discounting in this category** (if present) could erode these margins. The concentration also means weakness in tech demand would materially impact overall profitability.

---

### **4. Consumer Segment is the Most Profitable and Significantly Outperforms Corporate & Home Office**


**Finding:** Consumer segment generates **$134.1K in profit**, outperforming Corporate ($91.98K) by 31.4% and Home Office ($60.3K) by 122%. This indicates:

i. **Superior pricing power:** Consumer customers accept higher price points or resist discounting more effectively

ii. **Better demand matching:** Product-customer fit is stronger in the consumer channel

iii. **Operational efficiency:** Lower service costs or overhead in consumer operations(B2C) vs. business-to-business(B2B)

**Corporate and Home Office segments lag significantly, suggesting either**:

i. Price sensitivity in business segments is driving heavy discounts

ii. Product misalignment (e.g., offerings optimized for consumers, not businesses)

iii. Sales/service cost inefficiencies specific to B2B operations


### **5. Discounting is Inconsistent Across Products and Lacks Clear Performance Justification**

**Finding:** Discounting is heavily skewed toward Binders ($567, **36% of all discounts**), while other categories receive 75–80% less discount per transaction. This imbalance suggests:

i. **Reactive discounting:** Heavy markdowns on Binders are likely driven by excess inventory or weak demand, not strategic pricing

ii. **Lack of discount governance:** No clear limits, approval processes, or performance tracking

iii. **Margin leakage:** $567 in uncontrolled discounts represents pure profit loss without a corresponding uplift in volume.



### **6. Underperforming Products are Directly Reducing Overall Profitability**

**Finding:** Six product SKUs are collectively responsible for **over -$17,000 in losses**, representing **5.9% of total profit**. If these products operated at breakeven, profit would improve to $303.4K (+$17K, or +5.9% improvement). The loss-making products cluster in two categories:

i. **3D Printers (Technology):** Cubify and Lexmark models losing **$14.7K combined**, suggesting cost structure misalignment or price competitiveness issues

ii. **Conference Tables (Furniture):** Three models losing **$10.5K combined**, indicating either obsolete designs, high manufacturing costs, or market saturation

---

## Business Impact

### **Current Performance vs. Optimized Performance**

This analysis quantifies the difference between **actual 2022 performance** and **optimized performance** based on implementation of strategic recommendations.

#### **Scenario 1: Current State (2022 Actual)**
| Metric | Value |
|--------|-------|
| **Revenue** | $2.30M |
| **Profit** | $286.4K |
| **Profit Margin** | 12.5% |
| **Q4 Concentration** | 42% of annual sales |
| **Consumer Segment Profit** | $134.1K (46.8% of total) |
| **Loss-Making Products** | -$17K drag on profit |

#### **Scenario 2: Optimized State (Post-Recommendation Implementation)**
| Metric | Improvement | New Value |
|--------|-------------|-----------|
| **Remove Loss-Making Products** | +$17K | $303.4K |
| **Implement Discount Control (+3–5% margin)** | +$69–115K | $155.4–$186K profit uplift |
| **Expand Consumer Segment (+15–20% growth)** | +$20–27K | Additional profit |
| **Reduce Q4 Dependency (20–30% uplift in off-season)** | +$45–68K | Revenue smoothing + efficiency gains |
| **Strengthen Technology Category (+10–15% growth)** | +$84–126K | Additional profit |
| **COMBINED POTENTIAL** | **+$150–250K** | **$436K–$536K profit** |

#### **Key Improvements:**
1. **Profit Margin:** 12.5% → **18–22%** (44–76% improvement)
 
2. **Profit Growth:** $286.4K → **$436K–$536K** (52–87% improvement)
 
3. **Revenue Stability:** Q4 concentration from 42% → **35%** (more balanced)

4. **Loss Exposure:** -$17K → **$0** (elimination of underperformers)


## Recommendations

### 1: Eliminate Losses from Underperforming Products**

**Objective:** Remove or reprice loss-making SKUs to recover **$17,000+ in annual profit**, improving total profit margin by **0.7 percentage points** (12.5% → 13.2%).

Why it matters:
Loss-making SKUs contribute over -$17K in losses, directly reducing total profit.

Actions:

1. Review product margins within 30 days
2. Adjust pricing by 5–10% where feasible
3. Reduce inventory by 20–30%
4. Discontinue products after 30-60 days if losses persist

Target Outcome:

≥ 50% reduction in product losses

### **2. Implement Structured Discount Control & Governance**

**Objective:** Standardize discount allocation across products, enforce discount caps, and tie promotions to clear business outcomes.


Why it matters:
Uncontrolled discounting is compressing margins without clear returns.

Actions:

1. Set discount limits at 10–15% per category
2. Tie discounts to inventory reduction targets (~20%)
3. Track the performance of each promotion

Target Outcome:

+3–5% improvement in overall margin

### **3. Expand & Prioritize Consumer Segment**

**Objective:** Grow Consumer segment revenue and profit by **15–20%** over 12 months by increasing market penetration, repeat purchases, and average transaction value.
Why it matters:
Consumer segment delivers the highest profit ($134.1K).

Actions:

1. Increase marketing focus by 20–30%
2. Introduce loyalty programs
3. Bundle products to increase basket size

Target Outcome:

+15–20% growth in segment profit
+10% increase in average order value

### **4. Reduce Year-End Dependency & Smooth Revenue Across Months**

**Objective:** Flatten seasonal demand curve by boosting off-season (Q1–Q3) sales by **20–30%**, reducing Q4 concentration from **42% to ~35%** of annual revenue.
Why it matters:
Sales are concentrated in Q4, increasing dependency risk.

Actions:

1. Run campaigns in low months targeting 20–30% uplift
2. Introduce mid-year promotions
3. Use historical data for better demand planning

Target Outcome:

20–30% reduction in monthly sales volatility
*

### **5. Strengthen Core Technology Category **

**Objective:** Grow Technology category revenue by **10–15%** ($84–126K increase) while maintaining margin discipline, making it the primary profit driver.
Why it matters:
Technology contributes 36% of revenue and operates at high margins.

Actions:

1. Increase inventory by 15–25%
2. Focus marketing on top-performing tech products
3. Maintain pricing discipline to protect margins

Target Outcome:

+10–15% category revenue growth
---


## Conclusion

Tunia Technologies demonstrated **strong sales growth in 2022** ($2.30M revenue, +489% seasonal growth), but profit retention lagged significantly due to margin erosion, seasonal concentration, and underperforming products.

This analysis identifies **five high-impact strategic opportunities** that can collectively improve annual profit by **$150K–$250K (52–87% growth)** while reducing operational risk and improving decision-making visibility.

**Key Levers for Improvement:**
1. **Eliminate loss-making products** → +$17K profit
2. **Implement discount control** → +$69–115K profit (margin improvement)
3. **Expand Consumer segment** → +$20–27K profit
4. **Smooth seasonal demand** → +$45–68K profit
5. **Grow Technology category** → +$26–40K profit

With disciplined execution against these recommendations, Tunia Technologies can achieve **18–22% profit margins** (vs. current 12.5%), positioning the company for sustainable, profitable growth across African markets.

---

**Report Prepared By:** Adebisi Farouk Boluwatife  
**Role:** Business & Data Analyst  
**Date:** 2022 Analysis | 2025

