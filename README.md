# Sales Insights Dashboard

## 📌 Project Overview
AtliQ Hardware, a leading provider of computer hardware and peripherals, faced challenges in tracking sales performance across multiple regions in a rapidly changing market. 

This project delivers a **Power BI Business Intelligence solution** designed to provide real-time visibility into sales trends, customer performance, and regional profitability. By transforming raw transactional data into visual stories, this dashboard enables management to identify underperforming sectors and optimize their sales strategy.

---

## 🚀 Key Business Questions Answered
* **Revenue Analysis:** What is the total revenue and sales quantity across all regions?
* **Market Performance:** Which markets are driving growth and which need strategic intervention?
* **Customer Insights:** Who are our Top 5 customers by revenue and product volume?
* **Temporal Trends:** How is the revenue trending month-over-month and year-over-year?

---

## 🛠️ Technical Workflow (ETL & Modeling)

### 1. Data Cleaning & Transformation (Power Query)
Instead of a simple import, I performed a rigorous ETL process to ensure data "truth":
* **Currency Standardization:** Discovered inconsistent currency formats (INR and USD). I implemented a custom transformation column using DAX/M-Language logic: 
    > `if [currency] == "USD" then [sales_amount] * 83 else [sales_amount]`
* **Data Quality Assurance:** Performed "Column Profiling" across the **entire dataset** to ensure no null values or outliers were skewing the average calculations.
* **Data Filtering:** Removed "Null" and "Blank" market entries from the visual-level filters to ensure clean regional reporting.

### 2. Data Modeling
* **Time Intelligence:** Extracted `Year` and `Month` from the `cy_date` field to create a relational schema that supports drill-down analysis.
* **Calculated Measures:** Developed DAX measures for Total Revenue and Total Sales Quantity to allow for dynamic filtering.

---

## 📊 Dashboard Highlights
* **Total Revenue:** ₹ 984.81 Million
* **Total Sales Volume:** 2 Million Units
* **Top 5 Customers:** ElectricalSara Stores, Electricalslytical, Excel Store, Premium Stores, Nixon.
* **Interactive Visuals:** Bar charts for Revenue by Market and Revenue Trend lines for seasonal analysis.

---

## 📸 Screenshots

### Power BI Service Dashboard
![Dashboard_snap](https://github.com/user-attachments/assets/65e13e6d-941c-4b6c-a44f-d8588f157910)

### Power BI Desktop Report View
![Atliq_dashboard](https://github.com/user-attachments/assets/fd6ad3ec-8e3b-42b0-b169-95cf54e38790)

---

## 💡 Key Insights & Recommendations
* **Market Focus:** The dashboard identified specific regions where sales quantity is high but revenue is lower than expected, suggesting a need to review pricing strategies.
* **Retention:** Since the Top 5 customers contribute a significant portion of the revenue, AtliQ should implement loyalty programs or bulk-purchase discounts for these key accounts.
* **Growth Opportunity:** By analyzing the "Revenue Trend," management can now predict seasonal peaks and align inventory levels accordingly.

---

## 🧪 Tech Stack Used
* **Tool:** Power BI Desktop
* **Service:** Power BI Service (Cloud)
* **Data Source:** CSV / Excel
* **Transformation:** Power Query (M Language)
* **Calculations:** DAX (Data Analysis Expressions)
