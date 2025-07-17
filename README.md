# 📊 SQL Data Analytics Project

A hands-on, analytics-driven SQL project built to uncover insights from a modern data warehouse. This project uses advanced T-SQL queries to perform data exploration, segmentation, trend analysis, and KPI generation using dimensional modeling (star schema). It's ideal for showcasing data storytelling and analytical problem-solving skills.

---

## 📚 Table of Contents

* [🔍 Project Overview](#-project-overview)
* [🎯 Objectives](#-objectives)
* [🧱 Data Structure](#-data-structure)
* [📊 Analysis Modules](#-analysis-modules)
* [📈 Sample Insights](#-sample-insights)
* [🚀 How to Run](#-how-to-run)
* [🧰 Tech Stack](#-tech-stack)
* [🔮 Future Enhancements](#-future-enhancements)
* [📄 License](#-license)

---

## 🔍 Project Overview

This project simulates real-world analytics tasks performed over a cleaned and modeled SQL data warehouse. By leveraging structured queries, it enables business users and analysts to perform:

* Customer behavior analysis
* Product performance reviews
* Segmentation & cohort analysis
* Revenue and trend forecasting
* KPI dashboard reporting

The analysis is run on a **star schema** composed of dimension and fact tables in the `gold` layer.

---

## 🎯 Objectives

* Explore and validate database structures and metadata.
* Generate meaningful business metrics (sales, orders, customers).
* Perform segment-wise, time-series, and trend analyses.
* Build reusable analytical views and reports.
* Leverage SQL window functions for ranking and performance tracking.
* Enable customer and product segmentation.

---

## 🧱 Data Structure

**Star Schema Overview (Gold Layer):**

* `dim_customers` – Enriched customer demographics and CRM data
* `dim_products` – Product attributes, categories, cost, and life-cycle
* `fact_sales` – All transactional order data (sales, quantity, pricing)

Additional analytical views:

* `report_customers` – Customer-focused KPI summary and segmentation
* `report_products` – Product performance, ranking, and revenue classification

---

## 📊 Analysis Modules

The project contains well-documented scripts categorized as follows:

| 🔹 Module                  | 🧠 Purpose                                                                  |
| -------------------------- | --------------------------------------------------------------------------- |
| **Database Exploration**   | Understand schema and metadata using `INFORMATION_SCHEMA`                   |
| **Dimensions Exploration** | Extract unique values (e.g., countries, categories) for analysis            |
| **Date Range Analysis**    | Understand data availability over time using `MIN()`, `MAX()`, `DATEDIFF()` |
| **Key Metrics**            | Calculate totals, averages, and counts (e.g., sales, orders, products)      |
| **Magnitude Analysis**     | Analyze grouped metrics by category, gender, region, etc.                   |
| **Ranking Analysis**       | Use `TOP`, `RANK()`, `ROW_NUMBER()` to rank top/bottom performers           |
| **Cumulative Analysis**    | Track running totals and moving averages                                    |
| **Performance Trends**     | Perform YoY, MoM, and average deviation analysis using `LAG()`              |
| **Segmentation Analysis**  | Classify customers/products based on business logic                         |
| **Part-to-Whole Analysis** | Analyze category contribution to total revenue                              |
| **Customer Report View**   | Full customer profiling: orders, lifetime, recency, segmentation            |
| **Product Report View**    | Full product performance: quantity, customers, segment, revenue metrics     |

---

## 📈 Sample Insights

> 📌 A few example outputs this project can generate:

* "Top 10 customers generated 40% of revenue"
* "Products costing over \$1,000 contribute 60% of total sales"
* "Category ‘Mountain Bikes’ has the highest average monthly revenue"
* "Customer churn can be identified by tracking recency vs lifespan"
* "Segmented customers into `VIP`, `Regular`, and `New` based on behavior"

---

## 🚀 How to Run

1. Ensure the Gold Layer tables (`dim_customers`, `dim_products`, `fact_sales`) are available and populated.
2. Run each script independently or as part of an orchestrated SQL job in SSMS.
3. You may also convert key queries into **SQL views** for reporting or dashboarding purposes.
4. Use tools like **Power BI**, **Tableau**, or **Excel** to connect to these views for visualization.

---

## 🧰 Tech Stack

* **SQL Server / T-SQL**
* **Dimensional Modeling (Star Schema)**
* **Advanced SQL Functions**

  * Window Functions (`RANK()`, `LAG()`, `ROW_NUMBER()`)
  * Aggregations (`SUM()`, `AVG()`, `COUNT()`)
  * String, Date, and CASE logic

---

## 🔮 Future Enhancements

* Add parameterized stored procedures for dynamic filtering
* Build scheduled dashboards using Power BI
* Include predictive logic using SQL ML Services
* Introduce real-time metrics using SQL Change Data Capture (CDC)

---

## 📄 License

MIT License 

