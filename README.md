#  Sales Analysis Report – Power BI Project

## Project Overview

**Project Title:** Sales Analysis Report  
**Level:** Intermediate  
**Tool:** Microsoft Power BI  


This project demonstrates the use of Power BI to analyze sales performance and profitability across products, time periods, and sales channels. The interactive dashboard helps stakeholders track KPIs, identify trends, and make informed, data-driven business decisions.

## Objectives

- Analyze **Total Sales**, **Total Profit**, and **Profit Margin (%)** to evaluate overall business performance  
- Track **monthly sales and profit trends** to identify seasonality and growth patterns  
- Identify **top-performing products** based on sales value and profit contribution  
- Compare **sales performance across channels** (Store, Online, Reseller, Mobile Outlet)  
- Enable **state-level analysis** using location filters to assess regional performance  

![Library_project](https://github.com/BijoyBytes/retail-sales-analysis-powerbi/blob/main/TOOLS.png)
## 🧩 Dataset & Tables

### Fact Table

* **Sales_Data** – Transaction-level sales details including sales amount, profit, quantity, date, and foreign keys

### Dimension Tables

* **Sales_Channel** – Store, Online, Reseller, Mobile Outlet
* **Sales_Product** – Product-level information
* **Sales_Product_Sub_Cat** – Product sub-categories
* **Sales_Promotion** – Promotion and discount details
* **Sales_State** – State-level geographic data

---

## Data Preparation

* Removed duplicates and handled missing values
* Standardized date and numeric formats
* Created calculated columns using Power Query

---

## 🧠 Data Modeling

* Designed a **star schema** for efficient analysis
* Built relationships between fact and dimension tables
* Optimized model performance for reporting



## 📐 DAX Measures (KPIs)

```dax
• Total Sales = SUM(Sales_Data[Sales Amount])

• Total Profit = SUM(Sales_Data[Profit])

• Profit Margin % = DIVIDE([Total Profit], [Total Sales])

• Order Quantity = SUM(Sales_Data[Order Quantity])

• Total Products = DISTINCTCOUNT(Sales_Product[Product Name])

• Sales YoY % = Year-over-Year Sales Growth

• Profit YoY % = Year-over-Year Profit Growth
```

---

##  Dashboard Highlights

![Library_project](https://github.com/BijoyBytes/retail-sales-analysis-powerbi/blob/main/sales_dashbord.jpeg)

