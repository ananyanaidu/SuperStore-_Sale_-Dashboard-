
# 📊 Sales Performance Dashboard — Syntecxhub Internship

> **Data Analyst Internship | Week 1 | Syntecxhub**

---

## 📌 Overview

An interactive Power BI dashboard built on the SuperStore Sales Dataset to analyze sales performance across regions, categories, and time periods. The project covers end-to-end data analysis — from raw data cleaning to KPI creation and interactive reporting.

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| Power BI Desktop | Dashboard creation & visualization |
| DAX | KPI measures & time intelligence |
| Power Query (M) | Data cleaning & transformation |

---

## 📂 Dataset

- **Name:** SuperStore Sales Dataset
- **Format:** CSV
- **Total Orders:** 5,901
- **Date Range:** 2019 – 2021
- **Columns:** Order ID, Order Date, Ship Date, Ship Mode, Customer Name, Segment, Country, City, State, Region, Category, Sub-Category, Product Name, Sales, Quantity, Profit, Returns, Payment Mode

---

## 📊 Dataset Breakdown

| Field | Values |
|-------|--------|
| Categories | Furniture, Technology, Office Supplies |
| Regions | Central, East, South, West |
| Segments | Consumer, Corporate, Home Office |
| Payment Modes | Online, Cards, COD |

---

## ✅ Key Features

- ✔ Monthly sales trend analysis (3-year comparison — 2019, 2020, 2021)
- ✔ Quarterly sales trend — Q1 to Q4 year-wise comparison
- ✔ Top Sub-Categories by revenue
- ✔ Region-wise Revenue vs Profit comparison
- ✔ Category-wise sales breakdown (Donut chart)
- ✔ KPIs: Total Revenue, Total Profit, Profit Margin %, Quantity, Total Orders
- ✔ Interactive slicers: Region, Year, Category

---

## 📐 DAX Measures Used

```dax
Total Revenue = SUM('SuperStore Sales Dataset'[Sales])

Total Profit = SUM('SuperStore Sales Dataset'[Profit])

Total Orders = DISTINCTCOUNT('SuperStore Sales Dataset'[Order ID])

Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)

Revenue Last Year = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(DateTable[Date]))

```

---

## 🗂️ Files in This Repository

```
Syntecxhub_Sales_Performance_Dashboard/
│
├── Sales_Performance_Dashboard.pbix              # Power BI dashboard file
├── SuperStore_Sales_Dataset.csv      # Raw dataset
├── Dashboard_Screenshot.png          # Preview image
└── README.md                         # Project documentation
```

---

## 📸 Dashboard Preview

[Sales Dashboard]<img width="1123" height="633" alt="SuperStore_sales_ss" src="https://github.com/user-attachments/assets/576f27ac-afae-4dea-a35d-885c20865612" />



---

## 💡 Key Insights

1. **Office Supplies** is the highest revenue-generating category at 41.11%.
2. The **West region** leads in both revenue ($0.52M) and profit.
3. Sales show a clear **upward trend** from 2019 to 2021.
4. **Phones and Chairs** are the top-selling sub-categories.
5. Sales peak in **Q4** every year — especially November and December.
6. **South region** has the lowest revenue at $0.25M.
7. **Online** is the most used payment mode among customers.

---

## 👤 Author
Ananya A
