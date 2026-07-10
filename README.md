# Procurement & Supplier Performance Analytics Dashboard

Power BI project demonstrating procurement analytics, supplier performance evaluation, and operational KPI reporting using a synthetic manufacturing dataset.

---

## Overview

This project simulates a procurement analytics solution for a manufacturing company. It was built to demonstrate business intelligence concepts including:

- Star schema data modeling
- DAX measure development
- Executive KPI reporting
- Supplier performance analysis
- Operational performance monitoring
- Interactive cross-page filtering

---

## Dashboard Preview

### Executive Summary
![Executive Summary](screenshots/Executive%20Summary.png)

### Supplier Performance Analysis
![Supplier Performance Analysis](screenshots/Supplier%20Performance%20Analysis.png)

### Operational Performance Dashboard
![Operational Performance Dashboard](screenshots/Operational%20Performance%20Dashboard.png)

---

## Key Insights

- Electrical Components account for the highest procurement spend.
- Overall supplier score is 92.85, with an 89.10% on-time delivery rate.
- Average supplier lead time is 2 days.
- Defect rate remains low at 2.61%, indicating strong supplier quality.
- Monthly procurement spend peaks during April and September.

---

## Business Questions Solved

- Which suppliers have the highest performance scores?
- Which suppliers have the highest defect rates?
- Which procurement category contributes the most spend?
- How does procurement spending change month over month?
- Which suppliers require improvement based on KPIs?

---

## Dashboard Pages

### Executive Summary
- Total Spend, On-Time Delivery %, Defect Rate %, Average Lead Time, Overall Supplier Score (KPI cards)
- Monthly Spend Trend
- Spend by Category
- Top Suppliers by Spend
- Supplier Performance Scorecard (table)

### Supplier Performance Analysis
- Top 10 Suppliers by Performance Score
- Bottom 10 Suppliers by Performance Score
- Supplier Spend vs. Performance Score (scatter plot)
- Procurement Spend by Category (treemap)

### Operational Performance Dashboard
- Monthly Procurement Spend Ranking by Category (ribbon chart)
- Monthly On-Time Delivery Trend
- Procurement Spend by Defect Type

---

## Data Model

The report is built on a **star schema**:

- **Fact_PurchaseOrders** — transactional grain: PO date, spend, quantities
- **Dim_Supplier** — supplier name, country, supplier category
- **Product_Master** — product and category hierarchy
- **Dim_Quality** — defect type reference
- **Supplier Measure** — a dedicated, disconnected measures table holding all DAX calculations (Total Spend, On-Time Delivery %, Defect Rate %, Supplier Score, Avg Lead Time Days, Total Orders)

Raw source data starts as flat Excel files (see *Project Structure* below) and is cleaned and reshaped into the star schema above using Power Query.

---

## Skills Demonstrated

- Power BI & DAX
- Star schema data modeling
- Power Query (data cleaning & transformation)
- KPI dashboard design
- Procurement & supplier performance analytics
- Interactive, cross-page filtered dashboards
- Data visualization (treemap, scatter, ribbon chart, KPI cards)

---

## Project Structure

```
📂 screenshots/
   ├─ Executive Summary.png
   ├─ Supplier Performance Analysis.png
   └─ Operational Performance Dashboard.png

📄 Procurement & Supplier Performance Analytics Dashboard.pbix
📄 Supplier_Master.xlsx
📄 Product_Master.xlsx
📄 Purchase_Orders.xlsx
📄 Quality_Inspection.xlsx
📄 Supplier_Performance_Targets.xlsx
📄 Supplier Scorebook.xlsx
```

---

## Tech Stack

- Power BI Desktop
- Power Query
- DAX
- Microsoft Excel
- Star schema data modeling

---

## Project Type

**Personal Portfolio Project**

**Note:** The dataset used in this project is synthetic and was created to simulate a manufacturing procurement environment for learning and portfolio purposes.
