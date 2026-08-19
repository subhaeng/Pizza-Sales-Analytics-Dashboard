# BlinkIT Grocery Sales Dashboard 🛒

A single-page Power BI dashboard (`BlinKitDash.pbix`) that analyzes sales performance for **BlinkIT** ("India's Last Minute App") grocery data across outlets, item categories, and store attributes.

## Overview

This report gives a quick, visual snapshot of grocery sales performance — total sales, average sales, item count, and average customer rating — broken down by outlet type, outlet size, location tier, item category, and fat content. It's built as a single interactive page (`BLINKIT DASH`) with cross-filtering slicers so any visual can be sliced by location, outlet size, or item type.

## Data Source

- **Table:** `BlinkIT Grocery Data`
- Key fields used across the report: `Sales`, `Total Sales`, `Avg Sales`, `No Of Items`, `Avg Rating`, `Item Visibility`, `Item Type`, `Item Fat Content`, `Outlet Type`, `Outlet Size`, `Outlet Location Type`, `Outlet Establishment Year`.
- A supporting `Metrics` table drives a metric-selector slicer.

## Dashboard Contents

### KPI Cards
- **Total Sales** — sum of all sales
- **Average Sales**
- **Number of Items**
- **Average Rating**

### Visuals
| Visual | Type | What it shows |
|---|---|---|
| Fat Content | Donut chart | Total sales split by `Item Fat Content` (Low Fat vs Regular) |
| Fat by Outlet | Clustered bar chart | Total sales by `Outlet Location Type`, broken down by `Item Fat Content` |
| Item Type Sales | Bar chart | Total sales by `Item Type` (product category) |
| Outlet Establishment | Line chart | Total sales trend by `Outlet Establishment Year` |
| Outlet Size | Donut chart | Total sales split by `Outlet Size` (Small / Medium / High) |
| Outlet Location | Funnel chart | Sales by `Outlet Location Type` (Tier 1/2/3) |
| Outlet Type Summary | Pivot table | `Outlet Type` vs. Total Sales, No. of Items, Avg Sales, Avg Rating, and Item Visibility |

### Filters (Slicers)
- Metrics selector (switches the KPI card measure)
- Outlet Location Type
- Outlet Size
- Item Type

## Tech Stack

- **Tool:** Microsoft Power BI Desktop
- **File format:** `.pbix`
- **Modeling:** DAX measures (`Sum(Sales)`, `Avg Sales`, `Total Sales`, `Avg Rating`, etc.)

## How to Use

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).
2. Clone/download this repository.
3. Open `BlinKitDash.pbix` in Power BI Desktop.
4. Use the slicers on the report page to filter by outlet location, size, or item type.
5. Hover over any visual for tooltips with exact values.

> **Note:** If the underlying data source is not embedded, you may need to update the data source path via **Home → Transform Data → Data Source Settings** before refreshing.

## Repository Structure

```
.
├── BlinKitDash.pbix   # Power BI report file
└── README.md          # Project documentation
```

## License

Add your preferred license here (e.g., MIT).
##Dashboard
<img width="1136" height="746" alt="Home dash" src="https://github.com/user-attachments/assets/762dfe87-8d65-4b91-b373-1b1b2a730d92" />
<img width="1181" height="740" alt="B or W Sheller dash" src="https://github.com/user-attachments/assets/cd4de7a0-7437-41c7-8560-5edd970a8bf9" />



