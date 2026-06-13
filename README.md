#  Kevin Cookie Company — Sales Performance Analysis (2020–2022)

**Author:** Zainab R. Ogunjobi  
**Tools:** Microsoft Excel · Power BI  
**Dataset:** Kevin Cookie Company Internal Orders Data  
**Status:** ✅ Completed

---

## 📌 Project Overview

This project analyses **3 years of sales order data** from the Kevin Cookie Company — a fictional B2B cookie supplier selling to grocery stores, restaurants, and convenience chains across the United States. The goal was to uncover revenue trends, customer performance, profitability patterns, and the impact of rush shipments on business operations.

This was completed as a hands-on data analysis exercise using **Excel for data exploration and pivot analysis**, and **Power BI for interactive dashboard visualisation**.

---

##  Key Business Questions

1. How has total revenue and profit trended from 2020 to 2022?
2. Which customers generate the most revenue — and which are most profitable?
3. Does rush shipment status affect overall profitability?
4. Which months consistently record the highest and lowest sales?
5. What is the company's overall profit margin and cost structure?

---

## 📁 Repository Structure

```
kevin-cookie-sales-analysis/
│
├── data/
│   └── Kevin_Cookie_Company_Orders.xlsx     ← Raw orders + customer data (2 sheets)
│
├── analysis/
│   └── kevin_cookie_pivot_analysis.xlsx     ← Pivot tables, calculated fields & charts
│
├── dashboard/
│   └── kevin_cookie_dashboard.pbix          ← Power BI interactive dashboard
│   └── dashboard_preview.png                ← Screenshot of final dashboard
│
├── visuals/
│   ├── revenue_by_year.png                  ← Bar chart — annual revenue trend
│   ├── top_customers.png                    ← Bar chart — revenue by customer
│   ├── monthly_trend.png                    ← Line chart — monthly revenue pattern
│   └── rush_vs_nonrush.png                  ← Comparison chart
│
└── README.md
```

---

## 🗃️ Dataset Overview

| Detail | Info |
|--------|------|
| Source | Kevin Cookie Company (Practice Dataset) |
| Period | January 2020 — December 2022 |
| Total Records | 2,483 orders |
| Sheets | Orders, Customers |

**Orders Sheet Columns:**

| Column | Description |
|--------|-------------|
| Order ID | Unique order identifier |
| Customer ID | Links to Customers sheet |
| Rush Shipment | Whether order was rushed (Yes/No) |
| Cookies Shipped | Volume of cookies per order |
| Revenue | Order revenue in USD |
| Cost | Order cost in USD |
| Order Date | Date order was placed |

**Customers Sheet Columns:** Customer ID, Customer Name, Phone, Address, City, State, Zip, Country

---

## 🧹 Data Preparation Steps

Performed in **Excel** before analysis:

- ✅ Converted `Order Date` from serial number format to proper date format
- ✅ Created calculated column: `Profit = Revenue − Cost`
- ✅ Extracted `Month` and `Year` from Order Date for time-series analysis
- ✅ Used `VLOOKUP` to merge Customer Name from Customers sheet into Orders sheet
- ✅ Checked for duplicates using Excel's Remove Duplicates function — none found
- ✅ Verified no null values in key columns (Revenue, Cost, Order Date)
- ✅ Formatted currency columns to USD with 2 decimal places

---

## 📊 Key Findings & Insights

### 💰 Overall Business Performance

| KPI | Value |
|-----|-------|
| Total Revenue (3 Years) | **$6,417,240** |
| Total Profit (3 Years) | **$3,208,620** |
| Profit Margin | **50.0%** |
| Total Orders | **2,483** |
| Total Cookies Shipped | **1,283,448** |

> 🔍 **Insight:** A consistent 50% profit margin across all 3 years indicates a highly stable cost structure and disciplined pricing strategy.

---

### 📈 Revenue Trend by Year

| Year | Revenue |
|------|---------|
| 2020 | $2,036,940 |
| 2021 | $2,233,025 *(+9.6% YoY)* |
| 2022 | $2,147,275 *(-3.8% YoY)* |

> 🔍 **Insight:** Revenue grew strongly in 2021 but dipped slightly in 2022. This warrants further investigation — possible causes include customer churn, reduced order volumes, or market saturation.

---

### 👥 Top Customers by Revenue

| Rank | Customer | Revenue |
|------|----------|---------|
| 1 | Cascade Grovers | $1,886,790 |
| 2 | Quick Bite Convenience Stores | $1,560,410 |
| 3 | YT Restaurants | $1,354,915 |
| 4 | Park & Eat LLC | $1,190,530 |
| 5 | Acme Grocery Stores | $424,595 |

> 🔍 **Insight:** The top 4 customers account for over **93% of total revenue**, representing a significant customer concentration risk. Diversifying the customer base should be a strategic priority.

---

### 🚀 Rush vs. Non-Rush Shipments

| Type | Orders | Revenue |
|------|--------|---------|
| Rush | 1,248 | $3,206,495 |
| Non-Rush | 1,235 | $3,210,745 |

> 🔍 **Insight:** Rush and non-rush orders are almost perfectly split in both volume and revenue — suggesting rush shipments are not significantly more lucrative and may carry hidden costs (logistics, staffing) worth monitoring.

---

### 📅 Monthly Revenue Pattern

| Peak Months | Slow Months |
|-------------|-------------|
| June ($582,430) | February ($471,370) |
| May ($562,015) | April ($491,930) |
| September ($569,105) | March ($501,290) |

> 🔍 **Insight:** Mid-year (May–June) and early autumn (September) are the strongest sales periods. January and February are consistently slower — a potential window for promotional campaigns or new customer acquisition drives.

---

## 💡 Business Recommendations

1. **Reduce customer concentration risk** — top 4 customers represent 93%+ of revenue. A single lost account would have major business impact. Actively pursue new customer segments.

2. **Investigate 2022 revenue dip** — the 3.8% decline from 2021 deserves a root cause analysis. Review which customers reduced order volumes and why.

3. **Leverage peak seasons** — May, June, and September are peak months. Stock, staffing, and marketing resources should be scaled up ahead of these periods.

4. **Re-evaluate rush shipment pricing** — if rush orders carry higher logistics costs, pricing should reflect a premium. Currently, revenue per order is nearly identical to standard orders.

5. **Develop February–April promotion strategy** — the Q1 slowdown is consistent across all 3 years. Targeted offers or loyalty incentives during this period could smooth revenue distribution.

---

## 🛠️ How to Explore This Project

**Excel Analysis:**
1. Open `kevin_cookie_pivot_analysis.xlsx`
2. Navigate to the `Pivot Analysis` tab — revenue by customer, month, and year
3. Navigate to the `Charts` tab for visual summaries

**Power BI Dashboard:**
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Open `kevin_cookie_dashboard.pbix`
3. Use slicers to filter by Year, Customer, and Rush Shipment status

---

## 🚀 Skills Demonstrated

- ✅ Data cleaning and preparation in Excel
- ✅ Pivot table creation and calculated fields
- ✅ VLOOKUP for cross-sheet data merging
- ✅ KPI calculation (Revenue, Profit, Margin)
- ✅ Time-series trend analysis
- ✅ Power BI dashboard design
- ✅ Business insight generation from raw data

---

## 👩‍💻 About the Author

**Zainab R. Ogunjobi** is an Economics graduate and data analyst based in Lagos, Nigeria, with hands-on experience in financial reporting, data management, and business analysis.

🌐 [Portfolio](https://zainab-ogunjobi-va.netlify.app) · 💼 [LinkedIn](https://linkedin.com/in/ogunjobi-zainab) · 📧 [Email](mailto:Zainabogunjobir@gmail.com)

---

*Part of my Data Analytics Portfolio — feel free to fork or reach out with feedback!*
