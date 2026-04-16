## 📊 Amazon Sales Data Analysis — Power BI Dashboard
An end-to-end business intelligence project analysing 51,290 Amazon sales orders across 7 global markets, built entirely in Power BI with DAX measures, dynamic slicers, KPI cards, and Q&A visuals.
## 📁 Project Structure
```bash
amazon-sales-analysis/
│
├── ECOMM_DATA.xlsx          # Raw dataset (Orders, Returns, People sheets)
├── RUTUJA_POWERBI.pbix      # Power BI report file
├── Screenshots.pdf          # Dashboard preview screenshots
└── README.md
```
## 🎯 Objective
To analyse global Amazon sales performance and surface actionable insights across:

* Which ship modes generate the most revenue
* Which markets and countries are top performers
* Category-wise and city-wise sales distribution
* KPI tracking across Quantity, Sales, Profit, and Shipping Cost

## 📂 Dataset Overview


| Property | Details |
|---------|--------|
| Source | Amazon Global Sales Dataset |
| File | ECOMM_DATA.xlsx |
| Sheets | Orders, Returns, People |
| Total Orders | 51,290 |
| Time Period | 2011 – 2014 |
| Total Sales | $12.64 Million |
| Total Profit | $1.47 Million |
| Total Quantity | 178,312 units |
| Total Shipping Cost | $1.35 Million |

## Columns (Orders Sheet — 24 fields)
Row ID · Order ID · Order Date · Ship Date · Ship Mode · Customer ID · Customer Name · Segment · City · State · Country · Postal Code · Market · Region · Product ID · Category · Sub-Category · Product Name · Sales · Quantity · Discount · Profit · Shipping Cost · Order Priority

## 📊 Dashboard Features
KPI Cards

| Metric | Value |
|--------|-------|
| Sum of Quantity | 178,312 |
| Sum of Sales | $12.64M |
| Sum of Profit | $1.47M |
| Sum of Shipping Cost | $1.35M |

Visuals Built

| Visual | Description |
|--------|------------|
| 📌 KPI Cards | Top-level metrics for Sales, Profit, Quantity, and Shipping Cost |
| 🍩 Donut Chart — Sales by Market | Revenue share across APAC, EU, US, LATAM, EMEA, Africa, Canada |
| 🍩 Donut Chart — Sales by Category | Comparison of Furniture, Technology, and Office Supplies |
| 📊 Bar Chart — Sales by Country | Country-level revenue comparison |
| 📊 Bar Chart — Sales by City | City-level breakdown for granular insights |
| 📊 Bar Chart — Sales by Ship Mode | Standard Class leads at $7.58M (60% of revenue) |
| 🗺️ Map / State Visual | Geographic sales distribution by state |
| 🔍 Q&A Visuals (x3) | Natural language queries: state-wise, country-wise, and city-wise sales |
| 🎛️ Slicers | Filters for Category and Market selection |

## 🔑 Key Insights
🚚 Ship Mode Analysis

| Ship Mode | Total Sales | Share |
|-----------|------------|-------|
| Standard Class | $7.58M | ~60% |
| Second Class | $2.57M | ~20% |
| First Class | $1.83M | ~14% |
| Same Day | $0.67M | ~5% |
Standard Class is the dominant shipping method, contributing nearly 60% of all revenue.

🌍 Top 5 Countries by Sales
| Rank | Country | Sales |
|------|---------|-------|
| 1 | 🇺🇸 United States | $2.30M |
| 2 | 🇦🇺 Australia | $0.93M |
| 3 | 🇫🇷 France | $0.86M |
| 4 | 🇨🇳 China | $0.70M |
| 5 | 🇩🇪 Germany | $0.63M |

🏪 Top Markets by Revenue

| Market | Sales |
|--------|-------|
| APAC | $3.59M |
| EU | $2.94M |
| US | $2.30M |
| LATAM | $2.16M |
| EMEA | $0.81M |

📦 Category Breakdown

| Category | Sales |
|----------|-------|
| Technology | $4.74M |
| Furniture | $4.11M |
| Office Supplies | $3.79M |

## 🛠️ Tools & Techniques Used

| Tool / Feature | Usage |
|---------------|------|
| Power BI Desktop | Report building, data modelling, publishing |
| Power Query (M) | Data import, column type fixing, cleaning |
| DAX | Custom measures — Sales, Profit, KPI calculations |
| Slicers | Dynamic filtering by Category and Market |
| Q&A Visual | Natural language queries for self-service analytics |
| KPI Cards | At-a-glance business metrics |
| Donut & Bar Charts | Sales distribution across different dimensions |
| Excel (.xlsx) | Source data — Orders, Returns, People sheets |

## 🚀 How to Run This Project
Prerequisites

* Power BI Desktop (free) — version April 2024 or later recommended

Steps
1. Clone or download this repository
git clone https://github.com/your-username/amazon-sales-powerbi.git

2. Open the report
Double-click RUTUJA_POWERBI.pbix
OR open Power BI Desktop → File → Open → select the .pbix file

3. If prompted about data source path, update it:
Home → Transform Data → Data Source Settings → Change Source
Point to ECOMM_DATA.xlsx in your local folder

4. Click Refresh to reload data

## 📸 Dashboard Preview
See Screenshots.pdf for full dashboard screenshots including:

* Main KPI dashboard with slicers
* Q&A visual queries in action
* Country, city, and ship mode breakdowns

## 📈 DAX Measures Used
-- Total Sales
Total Sales = SUM(Orders[Sales])

-- Total Profit
Total Profit = SUM(Orders[Profit])

-- Total Quantity
Total Quantity = SUM(Orders[Quantity])

-- Total Shipping Cost
Total Shipping Cost = SUM(Orders[Shipping Cost])

-- Profit Margin %
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0) * 100

## 🧹 Data Preparation Steps

1. Loaded ECOMM_DATA.xlsx into Power BI via Power Query
2. Verified column data types (dates, decimals, text)
3. Handled null values in Postal Code and extra blank columns in Returns/People sheets
4. Created relationships between Orders, Returns, and People tables
5. Built DAX measures for all KPI cards
6. Designed report layout with slicers for interactive filtering

## 🤝 Connect
Rutuja Vanyalkar
*📧 rutujavanyalkar@gmail.com
*🔗 LinkedIn : https://www.linkedin.com/in/rutuja-vanyalkar29?utm_source=share_via&utm_content=profile&utm_medium=member_ios 

## 📄 License
This project is for portfolio and educational purposes.
Dataset used is publicly available Amazon sales sample data.
