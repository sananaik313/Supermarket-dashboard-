# Supermarket Sales Dashboard

An interactive sales analytics dashboard built in **Google Looker Studio**, visualizing transaction-level data from a supermarket chain with three branches across Myanmar (Yangon, Mandalay, Naypyitaw).

## Overview

The dashboard summarizes ~1,000 point-of-sale transactions to help stakeholders track revenue, customer behavior, and product performance across branches, product lines, and demographics.

**Key totals:**
- Total sales: **323.0K**
- Gross income: **15.4K**
- Average unit price: **55.7**
- Record count: **1,000 transactions**
- Total quantity sold: **6K units**
- Tax (5%) collected: **15K**

## Data Source

| File | Description |
|---|---|
| `Data.xlsx` | Raw transaction data (1,000 rows × 17 columns) feeding the Looker Studio report |
| `supermarket sale Dashboard.pdf` | Exported snapshot of the Looker Studio dashboard |

### Data Dictionary

| Column | Description |
|---|---|
| Invoice ID | Unique transaction identifier |
| Branch | Store branch code (A, B, C) |
| City | Branch city (Yangon, Mandalay, Naypyitaw) |
| Customer type | Member or Normal |
| Gender | Customer gender |
| Product line | Product category (Food and beverages, Sports and travel, Electronic accessories, Fashion accessories, Home and lifestyle, Health and beauty) |
| Unit price | Price per unit ($) |
| Quantity | Units purchased |
| Tax 5% | Sales tax applied |
| Total | Total transaction amount (incl. tax) |
| Date | Transaction date |
| Time | Transaction time |
| Payment | Payment method (Cash, Ewallet, Credit card) |
| cogs | Cost of goods sold |
| gross margin percentage | Gross margin % |
| gross income | Profit per transaction |
| Rating | Customer satisfaction rating (1–10) |

## Dashboard Sections

1. **KPI Cards** – Total sales, gross income, unit price, record count, quantity, and tax collected at a glance.
2. **Customer Sales** – Donut chart of Member (50.8%) vs. Normal (49.2%) customer split.
3. **Sales By City** – Bar chart comparing total sales across Naypyitaw, Yangon, and Mandalay.
4. **Unit Price vs Sales** – Dual-line comparison of average unit price and total sales by product line.
5. **Gross Income By Branch** – Pie chart showing gross income share for branches A, B, and C.
6. **Gross Income & Sales by Product** – Combo chart of gross income (bars) and record count (line) per product line.
7. **Gross Income by Gender & City** – Grouped bar chart breaking down gross income by gender across all three cities.

## Tools & Tech

- **Google Looker Studio** – report building and visualization
- **Google Sheets / Excel** – source data (`.xlsx`)
- **PDF export** – shareable static snapshot of the live report

## How to Reproduce

1. Upload `Data.xlsx` to Google Sheets or Google Drive.
2. In Looker Studio, create a new report and connect the Sheet as a data source.
3. Rebuild each chart per the **Dashboard Sections** above, using the relevant dimensions/metrics from the data dictionary.
4. Set the theme colors to the blue palette used in the original report for consistency.
5. Export to PDF via **File → Download → PDF** to generate a shareable snapshot.

## Notes

- Currency values are unlabeled in the source export; confirm currency (USD assumed) before publishing externally.
- Product line labels are truncated in some chart axes due to space constraints — full names are listed in the Data Dictionary above.
