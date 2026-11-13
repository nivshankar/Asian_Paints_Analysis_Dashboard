<div align="center">

# 🎨 Asian Paints Executive Sales Analytics Dashboard
### *Interactive Power BI Report — Executive Overview, Regional, Product, Dealer & Trend Analytics*

[![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-Measures_%26_KPIs-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Microsoft_Excel-Source_Data-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![Data Model](https://img.shields.io/badge/Data_Model-Relational_Design-7B2FBE?style=for-the-badge&logo=powerbi&logoColor=white)](https://powerbi.microsoft.com/)

<br/>

> *"Sales data tells the story of a business — visualise it well, and it becomes a strategy for growth."*

</div>

---

## 📋 Table of Contents

- [📌 Overview](#-overview)
- [🎯 Problem Statement](#-problem-statement)
- [✨ Key Features](#-key-features)
- [🏗️ Project Structure](#️-project-structure)
- [🔄 Project Workflow](#-project-workflow)
- [🔺 Page 1 — Executive Overview](#-page-1--executive-overview)
- [🔺 Page 2 — Regional Performance](#-page-2--regional-performance)
- [🔺 Page 3 — Product Analytics](#-page-3--product-analytics)
- [🔺 Page 4 — Dealer Performance](#-page-4--dealer-performance)
- [🔺 Page 5 — Trends & Executive Summary](#-page-5--trends--executive-summary)
- [🛠️ Tech Stack](#️-tech-stack)
- [📈 Results & Insights](#-results--insights)
- [🏆 Advantages](#-advantages)
- [📄 License](#-license)
- [👤 Author](#-author)
- [🙏 Acknowledgements](#-acknowledgements)

---

## 📌 Overview

The **Asian Paints Executive Sales Analytics Dashboard** is a five-page interactive Power BI report that gives sales and business leadership a consolidated view of **revenue and profit**, **regional performance**, **product and category analytics**, **dealer network performance**, and **trends with an executive summary**. Every page carries dropdown slicers, a left-hand navigation panel and KPI cards that show current values alongside previous-year (PY) comparisons.

All pages share a consistent navy-blue theme with the Asian Paints branding, a left navigation panel and a collapsible **Filters** pane.

This project is designed to:
- Track total revenue, profit, profit margin, orders and target achievement at an executive level
- Compare performance across Region › Zone › State › City using maps, tables and heatmaps
- Analyse product and category contribution, inventory turnover and revenue-versus-profit relationships
- Evaluate dealers by revenue, visit and order activity, dealer type and satisfaction rating
- Monitor monthly trends, cumulative YTD revenue, year-on-year growth and a forward-looking revenue forecast

---

## 🎯 Problem Statement

> **Objective:** Build an interactive Power BI dashboard that helps sales leaders and business heads monitor revenue and profitability, compare regions, products and dealers, and track growth trends against targets.

A paint manufacturer with **500 products**, **5,000 dealers** and **300K orders** across India needs to answer questions such as: *How is revenue growing against last year? Which regions, states and categories contribute most? Which products are the top performers? Which dealers and dealer types drive revenue? Are we on track against targets?*

| 📂 Page | 📄 Focus | 🔍 Core Question Answered |
|--------|---------|---------------------------|
| Executive Overview | Headline KPIs & scorecard | How is the business performing overall versus target and last year? |
| Regional Performance | Geography | Which regions and states drive revenue and margin? |
| Product Analytics | Products & categories | Which products and categories perform best? |
| Dealer Performance | Dealer network | Which dealers and dealer types contribute most, and how satisfied are they? |
| Trends & Executive Summary | Growth & outlook | How are revenue and profit trending, and what does the forecast say? |

---

## ✨ Key Features

| Feature | Description |
|--------|-------------|
| 🎛️ **Page-specific Slicers** | Date, Region, Hierarchy Level, Dealer Type, Product Category, Sub-Category, Product, Price Tier, State, Zone and City |
| 🏷️ **Dynamic KPI Cards** | Current value, previous-year value and change (green ▲ / red ▼ indicators) |
| 📉 **Trend Analysis** | Monthly line charts for revenue, profit, dealer visits and YoY growth, plus cumulative YTD revenue |
| 🎯 **Revenue vs Target** | Combo chart of revenue, target and target-achievement % by month and by region |
| 🍩 **Composition Charts** | Treemap and donut charts for category contribution and dealer satisfaction |
| 🗺️ **Geographic Maps** | Bubble maps and a filled map covering revenue and dealer locations across India |
| 🌡️ **Margin Heatmap** | State × Region matrix with conditional colour scale on profit margin |
| 🧮 **Executive Scorecard** | Category-level Revenue Achievement %, Profit Achievement %, Margin % and YoY growth |
| 🔮 **Revenue Forecast** | Forward-looking monthly revenue projection |
| 💡 **Insight Callouts** | Text summaries of the most important findings on key pages |
| 🧭 **Left Navigation** | Quick page switching across all five report pages |

---

## 🏗️ Project Structure

```
📦 Asian-Paints-Executive-PowerBI-Dashboard/
│
├── 📊 Asian_Paints_Executive_Dashboard.pbix  ← Power BI report file (5 pages)
├── 🗂️ Data/                                  ← Source data files (sales, products, dealers, regions, targets)
│
├── 📁 Assets/                                ← Screenshot assets for documentation
│   ├── 🖼️ Executive_Overview.png             ← Page 1 screenshot
│   ├── 🖼️ Regional_Performance.png           ← Page 2 screenshot
│   ├── 🖼️ Product_Analytics.png              ← Page 3 screenshot
│   ├── 🖼️ Dealer_Performance.png             ← Page 4 screenshot
│   └── 🖼️ Trends_Executive_Summary.png       ← Page 5 screenshot
│
└── 📄 README.md                              ← Project documentation
```

> **How to open:**
> ```
> 1. Install Power BI Desktop (free): https://powerbi.microsoft.com/desktop
> 2. Open Asian_Paints_Executive_Dashboard.pbix in Power BI Desktop
> 3. If prompted, re-point the data source to the files in the Data/ folder
> 4. Use the slicers on each page and the left navigation to explore
> ```

---

## 🔄 Project Workflow

```
Source Data  (Sales · Products · Dealers · Regions · Targets)
       │
       ▼  Import & clean in Power BI (Power Query)
  Data Model  (Date / Region / Zone / State / City / Product / Category / Dealer dimensions)
       │
       ├──▶  DAX Measures Created
       │     Total Revenue · Total Profit · Profit Margin % · Total Orders · Target Achievement %
       │     Revenue / Profit YoY % · YTD Revenue · Avg Revenue per Dealer
       │     Avg Dealer Satisfaction · Inventory Turnover · Revenue Contribution %
       │
       ├──▶  Page 1: Executive Overview
       │     ├── 2 top slicers (Date, Region) + 4 sidebar filters
       │     ├── 5 KPI cards (Revenue / Profit / Margin / Orders / Target Achievement)
       │     ├── Monthly revenue trend · Revenue vs Target combo chart
       │     └── Category treemap · Revenue map · Executive Scorecard
       │
       ├──▶  Page 2: Regional Performance
       │     ├── 2 top slicers (Date, Hierarchy Level) + 4 sidebar filters
       │     ├── 5 KPI cards
       │     ├── Filled map · Top Revenue by Region · Top 10 Revenue by State
       │     └── Revenue vs Target by Region · State × Region margin heatmap
       │
       ├──▶  Page 3: Product Analytics
       │     ├── 2 top slicers + 4 sidebar filters (Category / Sub-Category / Product / Price Tier)
       │     ├── 5 KPI cards (Revenue / Profit / Margin / Total Products / Avg Inventory Turnover)
       │     ├── Top 10 Product Revenue & Profit · Revenue by Category donut
       │     └── Inventory Turnover · Top Products table · Revenue vs Profit scatter
       │
       ├──▶  Page 4: Dealer Performance
       │     ├── 3 top slicers (Date, Hierarchy Level, Dealer Type) + 5 sidebar filters
       │     ├── 6 KPI cards (Revenue / Profit / Dealers / Orders / Avg Revenue per Dealer / Satisfaction)
       │     ├── Top 10 Dealers · Revenue distribution · Visits trend
       │     └── Satisfaction donut · Revenue by Dealer Type · Dealer map · Top 5 cities
       │
       └──▶  Page 5: Trends & Executive Summary
             ├── 2 top slicers + 4 sidebar filters
             ├── 6 KPI cards (YTD Revenue / YTD Profit / Margin / Revenue YoY / Profit YoY / Orders)
             ├── Revenue & Profit trends · YTD cumulative · Revenue Forecast
             └── Executive Scorecard · YoY Growth Trend · Executive Summary panel
```

---

## 🔺 Page 1 — Executive Overview

### 📝 1. Page Architecture

A high-level snapshot of business performance with headline KPIs, monthly revenue trends, target tracking, category contribution and a category-wise executive scorecard. Top slicers: **Date, Region**. Sidebar filters: **Product Category, Dealer Type, State, Zone**.

![Executive Overview Dashboard](Assets/Executive_Overview.png)

---

### 🗺️ 2. KPI Cards

| KPI Card | Value | Previous Year | Change |
|----------|-------|---------------|--------|
| 💰 **Total Revenue** | **₹7,017M** | ₹5,255M | ▲ 33.5% |
| 📈 **Total Profit** | **₹2,280M** | 1,708M | ▲ 33.5% |
| ➗ **Profit Margin %** | **32.50%** | 32.50% | ▼ 0.01% |
| 🧾 **Total Orders** | **300K** | 225K | ▲ 33.5% |
| 🎯 **Target Achievement %** | **9.29%** | 9.22% | ▲ 0.07% |

---

### 📊 3. Visuals

| Visual | Description |
|--------|-------------|
| **Revenue Trend (Monthly)** | Line chart from Jan 22 to Mar 23, fluctuating between roughly ₹131M and ₹150M per month |
| **Revenue vs Target (Monthly)** | Combo chart of revenue and target columns with a target-achievement % line ranging from about 8.66% to 9.67% |
| **Revenue by Category (Treemap)** | Putty ₹1,154.52M · Interior Emulsion ₹1,138.31M · Wood Finish ₹1,021.56M · Industrial Coating ₹1,020.38M · Primer ₹989.56M · Exterior Emulsion ₹891.07M · Waterproofing ₹801.2M |
| **Revenue by Region (Map)** | Bubble map showing revenue concentration across Indian locations |
| **Executive Scorecard (vs Target)** | Table with Revenue Achievement %, Profit Achievement %, Margin % and vs PY Growth % for each category, with a Total row |

---

### 📋 4. Executive Scorecard

| Category | Revenue Achievement % | Profit Achievement % | Margin % | vs PY Growth % |
|----------|----------------------|---------------------|----------|----------------|
| Exterior Emulsion | 9.55% | 15.26% | 32.54% | 34.38% |
| Industrial Coating | 9.50% | 15.23% | 32.51% | 33.31% |
| Interior Emulsion | 9.04% | 14.70% | 32.53% | 33.15% |
| Primer | 9.33% | 15.15% | 32.45% | 33.10% |
| Putty | 9.29% | 14.83% | 32.49% | 33.30% |
| Waterproofing | 9.21% | 15.14% | 32.48% | 33.66% |
| Wood Finish | 9.21% | 14.84% | 32.48% | 33.99% |
| **Total** | **9.29%** | **15.00%** | **32.50%** | **33.53%** |

---

### 💡 5. Key Insights (shown on dashboard)

- Total revenue grew **33.5%** to **₹7,017M** compared to the previous year
- Total profit reached **₹2,280M** at a steady margin of **32.50%**
- **Putty** is the largest category by revenue (₹1,154.52M), followed by Interior Emulsion (₹1,138.31M)
- **Exterior Emulsion** has the highest revenue achievement (9.55%) and the strongest YoY growth among the top performers (34.38%)
- Orders increased **33.5%** to **300K** compared to 225K last year

---

## 🔺 Page 2 — Regional Performance

### 📝 6. Page Architecture

Analyses performance across **Region › Zone › State › City**. Top slicers: **Date, Hierarchy Level**. Sidebar filters: **Product Category, Dealer Type, State, Zone**.

![Regional Performance Dashboard](Assets/Regional_Performance.png)

---

### 🗺️ 7. KPI Cards

| KPI Card | Value | Previous Year | Change |
|----------|-------|---------------|--------|
| 💰 **Total Revenue** | **₹7,017M** | ₹5,255M | ▲ 33.5% |
| 📈 **Total Profit** | **₹2,280M** | 1,708M | ▲ 33.5% |
| 🎯 **Target Achievement %** | **9.29%** | 9.22% | ▲ 0.07% |
| 🧾 **Total Orders** | **300K** | 225K | ▲ 33.5% |
| ➗ **Profit Margin %** | **32.50%** | 32.50% | ▼ 0.01% |

---

### 📊 8. Visuals

| Visual | Description |
|--------|-------------|
| **Revenue by Region (Filled Map)** | Choropleth map of India shaded by revenue intensity per state |
| **Top Revenue By Region** | Table of revenue and contribution by region — West leads (0.25), followed by Central, East and North (0.19 each) and South (0.18) |
| **Top 10 Revenue By State** | Mizoram (0.14), Himachal Pradesh (0.13), Rajasthan (0.11), West Bengal (0.10), Uttar Pradesh (0.10) and more |
| **Revenue vs Target By Region** | Combo chart with target-achievement % — West 9.34%, Central 9.05%, East 9.46%, North 9.44%, South 9.19% |
| **Top Revenue By Region (Heatmap)** | State × Region matrix of profit margin % (about 32.2%–33.0%) with red-to-green conditional formatting |

---

### 📋 9. Regional Revenue Contribution

| Region | Total Revenue (₹) | Contribution |
|--------|-------------------|--------------|
| West | 1,71,97,68,021.62 | 0.25 |
| Central | 1,35,86,39,553.84 | 0.19 |
| East | 1,35,81,16,701.11 | 0.19 |
| North | 1,31,91,70,883.82 | 0.19 |
| South | 1,26,09,01,979.31 | 0.18 |
| **Total** | **7,01,65,97,139.71** | **1.00** |

---

### 💡 10. Key Insights (shown on dashboard)

- **West** is the largest region, contributing about **25%** of revenue
- **Mizoram** (0.14) and **Himachal Pradesh** (0.13) lead the Top 10 states by revenue contribution
- **East** (9.46%) and **North** (9.44%) have the highest target achievement, while **Central** (9.05%) is the lowest
- Profit margins stay in a tight band across regions, with regional totals between **32.42%** and **32.54%**

---

## 🔺 Page 3 — Product Analytics

### 📝 11. Page Architecture

Comprehensive insights across **Product › Sub-Category › Product**. Top slicers: **Date, Hierarchy Level**. Sidebar filters: **Category, Sub-Category, Product, Price Tier**.

![Product Analytics Dashboard](Assets/Product_Analytics.png)

---

### 🗺️ 12. KPI Cards

| KPI Card | Value | Previous Year | Change |
|----------|-------|---------------|--------|
| 💰 **Total Revenue** | **₹7,017M** | ₹5,255M | ▲ 33.5% |
| 📈 **Total Profit** | **₹2,280M** | 1,708M | ▲ 33.5% |
| ➗ **Profit Margin %** | **32.50%** | 32.50% | ▼ 0.01% |
| 📦 **Total Products** | **500** | 500 | — |
| 🔁 **Avg Inventory Turnover** | **3%** | 3.30% | ▼ 0.01 |

---

### 📊 13. Visuals

| Visual | Description |
|--------|-------------|
| **Top 10 Product Revenue** | Horizontal bars — Product 399 (₹16.7M), Product 200 (₹16.0M), Product 222 (₹15.8M), Product 90 (₹15.7M), Product 162 (₹15.7M) |
| **Top 10 Product Profit** | Horizontal bars — Product 399 (₹5.4M), Product 200 (₹5.3M), Product 225 (₹5.2M), Product 162 (₹5.1M), Product 222 (₹5.1M) |
| **Revenue By Category** | Donut (₹7,017M centre) — Putty 16.5%, Interior Emulsion 16.2%, Wood Finish 14.6%, Industrial Coating 14.5%, Primer 14.1%, Exterior Emulsion 12.7%, Waterproofing 11.4% |
| **Inventory Turnover (x)** | Column chart — Primer, Exterior Emulsion and Putty at about 4x; Industrial Coating and Waterproofing at about 3x |
| **Top Products By Revenue** | Table with Product Name, Category, Revenue and Profit Margin % (about 32%–33%) |
| **Revenue vs Profit Scatter Analysis** | Scatter plot by category; products in the top-right quadrant are high performers |

---

### 💡 14. Key Insights (shown on dashboard)

- Products in the **top-right quadrant** of the scatter are high performers with higher revenue and profit
- Focus on **expanding high-margin products** and **improving low-margin, high-revenue products**
- **Asian Paint Product 399** leads both revenue (₹16.7M) and profit (₹5.4M)
- **Putty** is the largest revenue category (16.5% share) and **Waterproofing** the smallest (11.4%)

---

## 🔺 Page 4 — Dealer Performance

### 📝 15. Page Architecture

Tracks and analyses dealer performance across India. Top slicers: **Date, Hierarchy Level, Dealer Type**. Sidebar filters: **Dealer Type, Region, Zone, State, City**.

![Dealer Performance Dashboard](Assets/Dealer_Performance.png)

---

### 🗺️ 16. KPI Cards

| KPI Card | Value | Previous Year | Change |
|----------|-------|---------------|--------|
| 💰 **Total Revenue** | **₹7,017M** | ₹5,255M | ▲ 33.5% |
| 📈 **Total Profit** | **₹2,280M** | 1,708M | ▲ 33.5% |
| 🏪 **Total Dealers** | **5,000** | 5,000 | ▲ 0.0% |
| 🧾 **Total Orders** | **300K** | 225K | ▲ 33.5% |
| 👤 **Avg Revenue per Dealer** | **₹1,403K** | ₹1,051K | ▲ 33.5% |
| ⭐ **Avg Dealer Satisfaction** | **4.17** | 4.17 | ▲ 0.00 |

---

### 📊 17. Visuals

| Visual | Description |
|--------|-------------|
| **Top 10 Dealers By Revenue** | Horizontal bars — Dewan Inc (₹7.4M), Kala and S… (₹6.0M), Baral Ltd (₹5.5M), Dora Group (₹5.1M), Kala LLC (₹5.0M) |
| **Revenue per Dealer (Distribution)** | Column chart of dealer counts by revenue band — under 10 (99), 10–20 (4,881), 20–30 (20) |
| **Dealer Visits Trend (Monthly)** | Line chart of total visits (about 5.7K–6.4K) and total orders (about 2.0K–2.2K) from Jan 22 to Jan 23 |
| **Dealer Satisfaction Rating** | Donut across ratings 5 (Excellent) to 1 (Poor), dominated by Excellent and Very Good |
| **Revenue by Dealer Type** | Combo chart of revenue, profit and margin % across Distributor, Retail, Silver, Premium and Gold dealers |
| **Dealer Location Map** | Bubble map showing dealer revenue concentration across India |
| **Top 5 City By Dealer Revenue** | Bars led by Jamnagar (₹47M), Ghaziabad (₹46M) and Burhanpur (₹40M) |

---

### 💡 18. Key Insights (shown on dashboard)

- **Top-performing dealers** are highly satisfied and contribute significantly to revenue growth
- Top dealer types contribute the largest share of total revenue with higher margin performance
- **Jamnagar** leads in dealer revenue
- About **98%** of dealers (4,881 of 5,000) fall in the ₹10–20 revenue band, showing a very even dealer base
- Average dealer satisfaction holds steady at **4.17** out of 5

---

## 🔺 Page 5 — Trends & Executive Summary

### 📝 19. Page Architecture

Tracks performance trends, growth and future outlook for leadership reviews. Top slicers: **Date, Hierarchy Level**. Sidebar filters: **Region, Zone, Category, Dealer Type**.

![Trends & Executive Summary Dashboard](Assets/Trends_Executive_Summary.png)

---

### 🗺️ 20. KPI Cards

| KPI Card | Value | Previous Year | Change |
|----------|-------|---------------|--------|
| 💰 **YTD Revenue** | **₹7,017M** | ₹5,255M | ▲ 33.5% |
| 📈 **YTD Profit** | **₹2,280M** | 1,708M | ▲ 33.5% |
| ➗ **Profit Margin %** | **32.50%** | 32.50% | ▼ 0.01% |
| 📊 **Revenue YoY %** | **33.53%** | 50.27% | ▼ 16.7% |
| 📊 **Profit YoY %** | **33.51%** | 50.31% | ▼ 16.8% |
| 🧾 **Total Orders** | **300K** | 225K | ▲ 33.5% |

---

### 📊 21. Visuals

| Visual | Description |
|--------|-------------|
| **Revenue Trend (Monthly)** | Current-year vs prior-year revenue lines (Apr–Jan), current year ranging about ₹571M–₹605M with the peak in August |
| **Profit Trend (Monthly)** | Current-year vs prior-year profit lines, current year ranging about ₹185M–₹196M |
| **YTD Revenue (Cumulative)** | Cumulative revenue climbing steadily from ₹585M in April to about ₹5,278M by December, against prior-year cumulative |
| **Revenue Forecast** | Monthly forecast line projecting revenue between about ₹571M and ₹605M |
| **Executive Scorecard (vs Target)** | Category table of Revenue Achievement % and Profit Achievement % with a performance callout |
| **YoY Growth Trend (%)** | Revenue YoY % and Profit YoY % lines moving between roughly 32.6% and 34.4% |
| **Executive Summary Panel** | Four highlights — Strong Revenue Growth, Healthy Profitability, On Track with Targets, Positive Outlook |

---

### 💡 22. Key Executive Insights (shown on dashboard)

- **Strong Revenue Growth:** YTD revenue is **₹7,017M**, up **33.5%** compared to the previous year
- **Healthy Profitability:** YTD profit is **₹2,280M** with a margin of **32.50%**, showing strong improvement
- **On Track with Targets:** target achievement is above 100% across the organisation
- **Positive Outlook:** the forecast indicates continued growth in revenue over the next 6 months

---

## 🛠️ Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| 🟡 **Power BI Desktop** | Latest | Report authoring, data modelling, DAX and publishing |
| 📐 **DAX** | Built-in | Measures for revenue, profit, margin, YoY %, target achievement and YTD |
| 🧰 **Power Query** | Built-in | Data cleaning and transformation |
| 🎛️ **Slicers & Navigation** | Built-in | Dropdown filters, collapsible filter pane and page navigation |
| 🗺️ **Bing Maps Visual** | Built-in | Bubble maps and filled map of India |
| 🗂️ **Excel / CSV** | Source | Raw sales, product, dealer, region and target data |
| 🎨 **Report Theme** | Custom | Navy-blue branding with left navigation panel |

---

## 📈 Results & Insights

| Insight | Value |
|---------|-------|
| 💰 Total Revenue | **₹7,017M** (▲ 33.5% YoY) |
| 📈 Total Profit | **₹2,280M** (▲ 33.5% YoY) |
| ➗ Profit Margin | **32.50%** (stable vs PY) |
| 🧾 Total Orders | **300K** (▲ 33.5% YoY) |
| 🎯 Target Achievement | **9.29%** (▲ 0.07% vs 9.22%) |
| 🏆 Top Category by Revenue | **Putty** — ₹1,154.52M (16.5%) |
| 🌍 Largest Region | **West** — about 25% of revenue |
| 🗺️ Top State by Contribution | **Mizoram** — 0.14 |
| 📦 Total Products | **500** |
| 🥇 Top Product | **Asian Paint Product 399** — ₹16.7M revenue, ₹5.4M profit |
| 🏪 Total Dealers | **5,000** |
| 👤 Avg Revenue per Dealer | **₹1,403K** (▲ 33.5% YoY) |
| ⭐ Avg Dealer Satisfaction | **4.17** |
| 🏙️ Top City by Dealer Revenue | **Jamnagar** — ₹47M |
| 📊 Revenue YoY Growth | **33.53%** |
| 📅 Cumulative YTD Revenue (Dec) | **₹5,278M** |

---

## 🏆 Advantages

| Advantage | Detail |
|-----------|--------|
| 💼 **Executive Ready** | Branded, single-screen pages suitable for leadership reviews |
| ⚡ **Real-Time Filtering** | KPIs, charts, maps and tables respond to slicer changes instantly |
| 🔀 **Five-Lens View** | Overview, regional, product, dealer and trend analytics in one report |
| 🔎 **Drill-Down Capability** | Region › Zone › State › City and Category › Sub-Category › Product hierarchies |
| 🗺️ **Geographic Context** | Maps and heatmaps reveal regional concentration at a glance |
| 🎯 **Target Tracking** | Revenue-versus-target views by month, region and category |
| 💡 **Built-in Narrative** | Insight callouts and an executive summary translate numbers into plain language |
| 🖥️ **No Code Required** | Built entirely in Power BI Desktop and shareable as a `.pbix` file |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for full details.

```
MIT License — Free to use, modify, and distribute with attribution.
```

---

## 👤 Author

<div align="center">

### Neev Shankar

> *"Data transformed into structure becomes insight; insight transformed into strategy becomes growth."*

**🎓 Role:** Data Analyst | Power BI & Excel Specialist \
**📍 Location:** India \
**🛠️ Skills:** Power BI · DAX · Microsoft Excel · Data Visualisation · Dashboard Design · Data Modelling

</div>

---

## 🙏 Acknowledgements

- 📚 [Power BI Documentation](https://docs.microsoft.com/en-us/power-bi/) — Official Power BI Desktop and DAX reference
- 🟡 [Microsoft Power BI Community](https://community.powerbi.com/) — Dashboard design tips and DAX guidance
- 🎓 [SQLBI — DAX Guide](https://dax.guide/) — DAX function and measure reference
- 💬 [Stack Overflow Community](https://stackoverflow.com/) — Problem-solving support

---

<div align="center">

---

*Made with ❤️ and ☕ — Last updated: 13 November, 2026*

</div>
