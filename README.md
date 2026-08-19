# 🍕 Pizza Sales Dashboard — Power BI

An interactive Power BI dashboard analyzing a full year (Jan–Dec 2015) of pizza sales data. The report surfaces sales trends, order patterns, and best/worst performing products to support menu and operations decisions.

## 📊 Overview

The dashboard is built on a single fact table (`pizza_sales`) and presented across two report pages:

### 1. Home
A high-level KPI and trend overview, including:
- **KPI cards:** Total Revenue, Average Order Value, Total Pizzas Sold, Total Orders, Average Pizzas per Order
- **Busiest Days & Time:** Column chart of orders by day of week — highest volume on Fridays and Saturdays
- **Monthly Trend:** Area chart of orders by month — peaks in July and January
- **Sales by Category:** Donut chart of revenue by pizza category — Classic is the top category
- **Sales by Size:** Donut chart of revenue by pizza size — Large is the top-selling size
- **Category funnel:** Pizzas sold by category
- **Slicer:** Filter by pizza category

### 2. Best/Worst Sellers
A deep dive into product-level performance:
- **Top 5 / Bottom 5 Pizzas by Revenue**
- **Top 5 / Bottom 5 Pizzas by Quantity Sold**
- **Top 5 Pizzas by Orders**
- Same KPI card row and category slicer as the Home page for consistent filtering

## 🔑 Key Insights

- Orders peak on **weekend evenings** (Friday & Saturday)
- **July and January** are the highest-volume months
- The **Classic** category drives the most sales and orders overall
- **Large** pizzas contribute the most to total revenue
- The **Thai Chicken Pizza** generates the highest revenue
- The **Classic Deluxe Pizza** sells the highest total quantity and order count

## 🧮 Data Model

| Table | Purpose |
|---|---|
| `pizza_sales` | Core fact table with order-level pizza sales data |

**Key fields used across visuals:**
`pizza_name`, `pizza_category`, `pizza_size`, `Order Day`, `Order Month`

**Measures (DAX):**
- Total Revenue
- Total Orders
- Total Pizzas Sold
- Average Order Value
- Average Pizzas Per Order

## 🛠️ Tech Stack

- **Tool:** Microsoft Power BI Desktop
- **File:** `SQLPB.pbix`
- **Data source period:** January 2015 – December 2015

## 🚀 Getting Started

1. Clone or download this repository.
2. Open `SQLPB.pbix` in [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads).
3. Use the **category slicer** on either page to filter the entire report.
4. Navigate between **Home** and **Best/Worst Sellers** using the in-report page navigator.

## 📁 Repository Structure

```
├── SQLPB.pbix       # Power BI report file
└── README.md         # Project documentation
```

## 📌 Notes

- All monetary figures reflect the source dataset and are not adjusted for inflation or currency conversion.
- This report is intended for portfolio/demo purposes and uses a publicly available pizza sales dataset structure.

---

*Feel free to fork this project and adapt the dashboard for your own retail or F&B sales analysis.*
##Dashboard
<img width="1136" height="746" alt="Home dash" src="https://github.com/user-attachments/assets/762dfe87-8d65-4b91-b373-1b1b2a730d92" />
<img width="1181" height="740" alt="B or W Sheller dash" src="https://github.com/user-attachments/assets/cd4de7a0-7437-41c7-8560-5edd970a8bf9" />



