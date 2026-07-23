# GlobalShop International — Sales & Performance Dashboard

A Power BI dashboard built to give GlobalShop International leadership a single source of truth on revenue, product performance, customer behavior, and regional sales — replacing fragmented, delayed, and inconsistent manual reporting.

## Business Problem

GlobalShop International, a global bicycle and accessories retailer, was operating without reliable visibility into its own performance:

- **No product-level profitability visibility** — unclear which categories, subcategories, or individual products were profitable versus loss-making once stocking and shipping costs were factored in.
- **Delayed sales trend detection** — monthly reports arrived 2–3 weeks late, causing missed promotional windows and stockouts on fast-moving items.
- **No customer segmentation** — all 18K+ customers received identical treatment despite an assumed (unproven) revenue concentration among top customers.
- **No regional performance tracking** — country-level growth, decline, and opportunity areas were invisible to sales leadership.
- **No fulfilment/delivery performance measurement** — rising delivery complaints with no way to isolate whether delays originated at order, warehouse, or carrier stage.
- **Untrusted, inconsistent data** — missing values, inconsistent country naming, unassigned product categories, and unreliable date fields meant different people got different numbers from the same source.

## Objective

Build a self-service Power BI dashboard that gives stakeholders a trusted, real-time view of revenue, profit, product performance, and customer/regional trends — without waiting on manual reporting cycles.

## Dashboard Pages

| Page | Purpose |
|---|---|
| **Executive Summary** | Company-wide KPIs — revenue, profit, margin, orders, customers, AOV — plus top products by revenue, revenue by country, revenue trend, and category-level revenue/margin split |
| **Product Performance** | Product-level revenue and profit, performance classification (High Performer vs. Needs Attention by margin %), top/bottom 10 products by profit |
| **Customer Analytics** | Customer segmentation and behavior (see file) |
| **Regional Performance** | Country/region-level revenue, growth, and trend breakdown (see file) |

## Key Findings

- Total revenue: **$29.4M** across **28K orders** and **18K customers**, at a **39.8%** overall profit margin (AOV: **$1.06K**).
- The **Mountain-200** series occupies 8 of the top 10 revenue-generating products.
- **United States** drives 31% of total revenue, followed by Australia (17%) and UK (12%).
- Revenue grew **130%** from 2011 ($7.1M) to 2013 ($16.3M); 2014 data is partial (January only).
- **Bikes** generate 87% of total revenue but the lowest category margin (39.2%); **Accessories** carry the highest margin (62.8%) despite low revenue share.
- Of 295 products, a defined subset falls below the 20% margin threshold and is flagged for review under the "Needs Attention" classification.

## Data Model & Methodology

- Star-schema semantic model built in Power BI (Fact: Orders/Sales; Dimensions: Product, Customer, Date, Geography).
- Performance classification: products with margin ≥ 40% labeled **High Performer**; below 20% labeled **Needs Attention**.
- Data cleaning addressed inconsistent country naming, missing category assignments, and unreliable date fields prior to modeling.

## Tools Used

- **Power BI** — data modeling, DAX measures, dashboard design
- **DAX** — KPI calculations, margin classification, trend measures

## Repository Contents

```
├── GlobalShop_Dashboard.pbix     # Power BI source file
├── screenshots/                  # Dashboard page exports
└── README.md
```

## How to Use

1. Clone the repository.
2. Open `GlobalShop_Dashboard.pbix` in Power BI Desktop.
3. Refresh the data connection if source files have moved.
4. Use the top navigation buttons to move between Executive Summary, Product Performance, Customer Analytics, and Regional Performance.

## Author

**Nnadika Nnetachukwu Peace**
Data Analytics Coach & Consultant, SharaShell Technology Limited
[GitHub](https://github.com/Peaceyoung64) · [LinkedIn](https://www.linkedin.com/in/nnadika-nnetachukwu-peace-385918396/)
