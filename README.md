# 🛒 Supermarket Sales Performance Dashboard

> A Power BI dashboard analyzing supermarket sales, profitability, and customer behavior across multiple branches — built around two focused views: financial performance and operations/customer behavior.

---

## 🖼️ Dashboard Preview

**View 1 — Sales & Performance Overview**
![Sales Dashboard](./assets/page1_sales_performance.png)

**View 2 — Operations & Customer Insights**
![Operations Dashboard](./assets/page2_operations_customer.png)

---

## 🚀 Project Overview

This project analyzes 2019 transactional data from a multi-branch supermarket chain operating across three regions — Naypyitaw, Yangon, and Mandalay. I designed it around two clear lenses: financial performance on one view, operations and customer behavior on the other — the way real retail BI reporting is typically structured.

The core question driving this project: **does high revenue actually mean high profitability?** The data says no — and that gap is what the dashboard is built to expose.

---

## 🎯 Business Problem Statement

Retail leadership needs visibility into:
1. Which regions and product categories drive the most profit (not just revenue)
2. When peak transaction activity occurs, to optimize staffing
3. How payment method choice affects basket size and revenue mix
4. Which branches deliver the strongest customer satisfaction
5. Demographic and behavioral patterns to guide marketing spend

---

## 🛠️ Tools & Tech Used

| Layer | Tools Used |
|---|---|
| **BI & Visualization** | Power BI Desktop — interactive dashboard with KPI cards, trend charts, and cross-filtering |
| **Data Transformation** | Power Query — data cleaning, null handling, type transformations |
| **Analytical Engine** | DAX — custom measures for Profit Margin %, Average Order Value, Unique Order counts |
| **Data Modeling** | Relational model with a Calendar dimension table |
| **Filtering** | Cross-page filters synced across Products, City, Customer Type, Gender, and Rating |

---

## 📈 View 1: Sales & Performance Insights

**KPIs:** Total Sales ($322.97K) · Total Profit ($15.38K) · Profit Margin (4.76%) · Avg Order Value ($322.97) · Unique Customers (1K)

- **Daily Revenue Trend** — tracks cumulative revenue growth from Jan–Mar 2019
- **Regional Revenue vs. Profitability** — compares revenue and profit across Naypyitaw, Yangon, and Mandalay to identify where margins hold up and where they don't
- **Weekly Sales & Profit Analysis** — correlates sales volume with profit over time
- **Revenue by Product Category** — ranks 6 categories by revenue (Food & Beverages leads at $56.14K)

---

## 📈 View 2: Operations & Customer Insights

- **Peak Transaction Hours** — identifies highest-traffic hours for staffing decisions
- **Weekly Order Volume** — shows Friday/Saturday as peak order days
- **Revenue Share by Payment Method** — Cash (34.74%), E-wallet (34.06%), Credit Card (31.2%)
- **Avg Basket Size by Payment Type** — compares transaction value across Cash, Credit Card, and E-wallet users
- **Customer Satisfaction (CSAT) by Branch** — branch-level rating comparison (Branch C leads at 7.1)
- **Customer Demographics by Gender** — near-even split (Female 50.1% / Male 49.9%)
- **Top 5 Revenue-Generating Transactions** — drill-down table of highest-value individual transactions

---

## 💡 Key Business Insights

### 1. High Revenue Doesn't Guarantee High Profit
A 4.76% profit margin on $322.97K in sales shows top-line growth isn't automatically translating to the bottom line.

**Recommendation:** Conduct margin analysis by individual product line, not just category, to find where discounting or cost overhead is eroding profit.

### 2. Regional Revenue Doesn't Match Regional Profitability
All three regions show comparable revenue (~100K–111K each), but profitability diverges sharply — pointing to cost differences worth investigating at the regional level.

**Recommendation:** Compare operating costs (logistics, staffing) across regions to identify where margin is being lost.

### 3. Payment Methods Are Nearly Evenly Split — But Not Equal in Value
Cash (34.7%), E-wallet (34%), and Credit Card (31%) are close in share, but cash transactions consistently have the largest average basket size ($326.18).

**Recommendation:** Promote digital payment incentives without removing cash options, since cash customers are currently the highest-value segment.

### 4. Peak Hours Are Predictable and Actionable
Friday and Saturday drive the highest weekly order volume (164 and 133 orders respectively).

**Recommendation:** Align staff scheduling with these peak days and hours to reduce wait times and support CSAT scores.

---

## 📂 Repository Structure

supermarket-sales-dashboard/
│
├── Supermarket_Sales.pbix          # Power BI Dashboard file
├── Data/
│   └── supermarket_sales.csv       # Raw dataset
├── assets/
│   ├── page1_sales_performance.png
│   └── page2_operations_customer.png
└── README.md
