# Interactive Sales Performance Dashboard (Power BI & Star Schema)

## 📌 Project Overview
This project focuses on the design and implementation of an enterprise-grade Business Intelligence (BI) dashboard using **Power BI**. By transforming raw transactional data into a highly structured data warehouse model, this solution enables interactive exploration and deep-dive analysis of organizational sales performance across multiple strategic dimensions: products, customers, regions, and time hierarchies.

## 🏗️ Data Architecture & Modeling
The backbone of this project is a robust **Star Schema** designed to optimize query performance and ensure intuitive data exploration. 

The architecture consists of:
* **Fact Table:** `FactOrders` (Stores transactional metrics: Sales, Quantity, Discount, Profit, Order/Shipping Dates).
* **Dimension Tables:** * `DimCustomer` (Demographics, segments, and customer details)
    * `DimProduct` (Product categorization, sub-categories, and naming)
    * `DimRegion` (Geographical mappings and regional hierarchies)
    * `DimDate` (Official marked calendar table enabling time-intelligence functions)

## ⚡ Key Features & Insights
* **Dynamic Performance KPIs:** Instant tracking of Total Revenue, Units Sold, Average Selling Price, and Profit Margins.
* **Time-Intelligence Insights:** Advanced DAX metrics highlighting sales trends and growth patterns over quarters and fiscal years.
* **Advanced Interactivity:** Synchronized slicers, cross-filtering, and diagnostic drill-downs to pinpoint operational bottlenecks or high-performing customer segments.
* **Data Governance:** Implementation of **Row-Level Security (RLS)** to guarantee controlled, role-based data access for stakeholders.

## 🛠️ Tech Stack & Tools
* **Power BI Desktop:** Data modeling, DAX engineering, and dashboard virtualization.
* **Power Query (M Language):** Extract, Transform, Load (ETL) processing and type validations.
* **Data Source:** Relational CSV datasets (`FactOrders`, `DimCustomer`, `DimProduct`, `DimRegion`, `DimDate`).

`## 📊 Dashboard Preview`
<img width="927" height="544" alt="image" src="https://github.com/user-attachments/assets/099713dd-5857-4af8-8d0d-dba148beb4fd" />


## 📂 Repository Structure
```text
├── Data/
│   ├── FactOrders.csv
│   ├── DimCustomer.csv
│   ├── DimProduct.csv
│   ├── DimRegion.csv
│   └── DimDate.csv
├── powerbi-sales-analytics-star-schema.pbix       # Core Power BI Project File
├── powerbi-sales-analytics-star-schema.pdf        # Detailed Project Report & Documentation
└── README.md
