# Car Sales Data Dashboard (Excel)

An interactive **Excel dashboard** built from a car sales dataset of roughly 10,000 records. It uses PivotTables and PivotCharts to answer key business questions: which brands earn the most, how revenue has changed over the years, and which models sell best.

---

## Project Overview

| Item | Details |
|------|---------|
| **Tool** | Microsoft Excel (PivotTables, PivotCharts) |
| **Dataset size** | ~10,000 sales records |
| **Total revenue analysed** | ~18.22 Billion |
| **Period covered** | 2019 – 2025 |
| **Workbook sheets** | `data` (raw data), `Sheet2` (pivots and charts), `Sheet1` |

---

## Dataset Description

The `data` sheet holds one row per car sale with these columns:

| Column | Description |
|--------|-------------|
| `SaleID` | Unique sale identifier |
| `VIN` | Vehicle Identification Number |
| `Company Name` | Car brand / manufacturer |
| `Model` | Car model |
| `Year` | Manufacturing year |
| `Color` | Car colour |
| `FuelType` | Petrol / Diesel / Electric / CNG / Hybrid |
| `Transmission` | Manual / Automatic / CVT |
| `Price` | Sale price (used as revenue) |
| `Mileage_km` | Kilometres driven |
| `Dealer` | Selling dealership |
| `State` | State of sale |
| `SaleDate` | Date of sale |
| `CustomerName` | Customer name |
| `CustomerEmail` | Customer email |
| `Customer_rating` | Customer rating |
| `Notes` | Service / warranty / exchange remarks |
| `Finance` | Whether the purchase was financed (Yes / No) |

> Some fields contain placeholder values such as `not provided`. These were left as-is, so consider cleaning them before any deeper analysis.

---

## Dashboard Charts & Insights

### 1. Top 5 Companies by Brand
![Top 5 Company by Brand](images/top5_company_by_brand.png)

- **Audi** leads with about **2.22B** in revenue.
- **Mercedes-Benz (2.05B)** is a close second, followed by **BMW (1.75B)**, **Ford (1.49B)** and **Volkswagen (1.48B)**.

---

### 2. Revenue by Company
![Revenue by Company](images/revenue_by_company.png)

- Compares revenue across **all 12 brands** (bar chart with a trend line).
- Audi and Mercedes-Benz are clearly ahead of the rest.
- **Mahindra & Mahindra (~1.13B)** has the lowest revenue among the listed brands.

---

### 3. Market Share by Brands (%)
![Market Share by Brands](images/market_share_by_brands.png)

- Shows each brand's share of total revenue as a 3D pie chart.
- Approximate shares: **Audi 12%**, **Mercedes-Benz 11%**, **BMW 10%**, **Ford / Hyundai / Tata Motors / Toyota / Volkswagen ~8% each**, **Honda / Kia / Maruti Suzuki ~7% each**, **Mahindra & Mahindra 6%**.
- No single brand dominates; the market is fairly evenly spread.

---

### 4. Yearly Revenue Trend
![Yearly Revenue Trend](images/yearly_revenue_trend.png)

| Year | Revenue (B) |
|------|-------------|
| 2019 | 2.64 |
| 2020 | 2.87 *(peak)* |
| 2021 | 2.72 |
| 2022 | 2.75 |
| 2023 | 2.68 |
| 2024 | 2.69 |
| 2025 | 1.87 |

- Revenue stayed stable at around **2.6–2.9B** per year from 2019 to 2024.
- **2020** was the peak year.
- **2025** shows a sharp drop to **1.87B**, possibly because the year's data is incomplete. Verify this before drawing conclusions.

---

### 5. Top 10 Models by Share
![Top 10 Models by Share](images/top10_models.png)

- **Audi Q5 (1.09B)** and **Mercedes C-Class (1.02B)** are the top two models, each above 1B.
- The remaining models (3 Series, E-Class, Carens, A4, Polo, Endeavour, A6, Figo) sit in the **0.52B – 0.69B** range.

---

## Key Takeaways

- Premium German brands (**Audi, Mercedes-Benz, BMW**) lead on revenue.
- Revenue was stable across 2019–2024, with a notable dip in 2025.
- A few flagship models (**Q5, C-Class**) contribute disproportionately to revenue.
- Brand market share is fairly balanced, with no monopoly.

---

## Skills & Techniques Used

- Data cleaning and preparation in Excel
- PivotTables for aggregation (Sum of Price by brand / year / model)
- PivotCharts: column + line combo, 3D pie, line chart, horizontal bar
- Dark-themed dashboard styling and data labels

---

## Repository Structure

```
├── README.md
├── Data_dashboard.xlsx      # Excel workbook (data + pivots + charts)
└── images/
├── top5_company_by_brand.png
├── revenue_by_company.png
├── market_share_by_brands.png
├── yearly_revenue_trend.png
└── top10_models.png
```

---

## How to Use

1. Download or clone this repository.
2. Open `Data_dashboard.xlsx` in Microsoft Excel.
3. Go to **Sheet2** to explore the pivot tables and charts.
4. Use the pivot filters to slice the data by brand, year or model.

---
