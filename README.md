# Operations & Inventory MIS Automation Dashboard

## 📌 Project Overview

An automated Excel-based Management Information System (MIS) designed to monitor
orders, inventory, purchasing activity, regional performance, and operational delays.

The solution transforms raw operational data using Power Query, calculates
management KPIs using Excel formulas, presents insights through an interactive
dashboard, and uses VBA automation for one-click MIS refresh.

## 🔑 Key Highlights

- Automated data cleaning and transformation using Power Query
- Centralized MIS KPI reporting
- Order and dispatch performance monitoring
- Inventory stock and shortage analysis
- Purchase value and quantity tracking
- Region-wise operational performance analysis
- Dynamic management insights and recommendations
- One-click MIS refresh using VBA
- Automated Last Updated timestamp

## 🎯 Business Problem

The organization required a centralized reporting solution to monitor
day-to-day operational performance across orders, inventory, and purchasing.

Manual reporting made it difficult to quickly identify pending orders,
dispatch delays, stock shortages, purchasing trends, and regional performance
issues.

This project was developed to provide management with a centralized,
automated, and easy-to-use MIS dashboard for operational decision-making.

## 🎯 Project Objectives

- Monitor total order volume and order status
- Track pending and delayed orders
- Measure dispatch and on-time performance
- Monitor closing stock and inventory availability
- Identify low-stock and out-of-stock items
- Track purchase value and purchase quantity
- Analyze operational performance by region
- Identify regions with higher delay rates
- Provide actionable management insights
- Automate MIS data refresh using VBA
- Display the latest dashboard refresh timestamp

- ## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | MIS reporting and dashboard |
| Power Query | Data cleaning and transformation |
| Excel Formulas | KPI calculations and business logic |
| Excel Charts | Data visualization |
| VBA | One-click refresh automation |


## 🏗️ Data Architecture

The project follows a simple ETL-style workflow:

```text
Raw Operational Data
        ↓
Power Query
        ↓
Data Cleaning & Transformation
        ↓
MIS Summary
        ↓
KPI Calculations & Regional Analysis
        ↓
Excel Dashboard
        ↓
VBA One-Click Refresh
```

### Data Sources

The solution uses three operational datasets:

| Dataset | Description | Records |
|---|---|---:|
| Orders | Order and dispatch information | 1,000 |
| Inventory | Product stock information | 32 |
| Purchase | Supplier and purchasing information | 300 |

### Data Processing Workflow

1. Load raw operational datasets into Excel.
2. Import datasets using Power Query.
3. Clean and transform the data.
4. Create required calculated fields.
5. Load transformed data into Excel tables.
6. Build MIS summary calculations.
7. Create KPI metrics and regional analysis.
8. Build the management dashboard.
9. Add dynamic business insights.
10. Automate the refresh process using VBA.

## 📊 Key Performance Indicators

| KPI | Definition |
|---|---|
| Total Orders | Total number of orders received |
| Dispatched Orders | Number of orders successfully dispatched |
| Pending Orders | Orders that are still pending |
| Delayed Orders | Orders classified as delayed |
| On-Time % | Percentage of dispatched orders completed on time |
| Total Quantity | Total quantity associated with orders |
| Closing Stock | Total available inventory stock |
| Low Stock Items | Number of products below the defined stock threshold |
| Out of Stock Items | Number of products with zero available stock |
| Total Purchase Value | Total monetary value of purchases |
| Total Purchase Quantity | Total quantity purchased |


## 📊 Dashboard Preview

The dashboard provides a centralized view of operational performance,
inventory availability, purchasing activity, regional performance,
and management insights.

![Operations & Inventory MIS Dashboard](Screenshot/Operation%20Inventory%20Dashboard.png)


## 📈 Business Insights

Based on the analysis performed in the MIS dashboard:

### 1. Regional Order Performance

North is the highest-volume region with **279 orders**, while East has
the lowest order volume with **234 orders**.

### 2. Regional Delay Performance

West has the highest delayed-order rate at **8.94%**, indicating a higher
operational delay risk compared with other regions.

East has the lowest delayed-order rate at **8.12%**.

### 3. Overall Operational Performance

The business processed **1,000 orders**, with **86 delayed orders** and
an overall on-time performance of **88.27%**.

### 4. Inventory Risk

The dashboard identifies **6 low-stock items** and **2 out-of-stock items**,
highlighting inventory areas that require monitoring.

## 💡 Business Recommendations

- Investigate dispatch and operational bottlenecks in the West region.
- Review warehouse and logistics processes contributing to delays.
- Monitor low-stock products to reduce the risk of stockouts.
- Prioritize replenishment for out-of-stock items.
- Continue monitoring regional delay rates through the automated MIS.
- Use the one-click refresh process to keep management reporting current.

## ⚙️ Automation

The reporting workflow was automated using Excel VBA.

### One-Click MIS Refresh

The dashboard includes a **Refresh MIS** button that triggers the
Power Query refresh process.

The automated workflow is:

1. User clicks **Refresh MIS**.
2. Power Query connections are refreshed.
3. MIS summary calculations are updated.
4. Dynamic KPI cards reflect the latest values.
5. Regional charts update with refreshed data.
6. Management insights update automatically.
7. The **Last Updated** timestamp is refreshed.

### VBA Automation

A custom VBA macro was developed to simplify the reporting process
and reduce repetitive manual refresh activities.

This allows the MIS report to be refreshed through a single dashboard
button instead of manually refreshing individual queries.

## 📁 Project Structure

```text
operations-inventory-mis-automation/
│
├── README.md
├── Operations_Inventory_MIS_Dashboard.xlsm
└── MISdashboard.png
```

### Main Components

- **README.md** — Project documentation
- **Operations_Inventory_MIS_Dashboard.xlsm** — Complete automated Excel MIS solution
- **Mis_dashboard.png** — Dashboard preview

## 🚀 Future Improvements

Potential enhancements for the next version include:

- Automated email distribution of the MIS report
- Scheduled report generation
- Power BI integration
- Advanced inventory forecasting
- Supplier performance analysis
- Automated exception alerts
- Role-based management reporting
