# Global-Superstore-SQL-Powerbi
End-to-end SQL data warehouse project with Power BI dashboard using the Global Superstore dataset.

---

## 📌 Project Overview

This project was built as my first end-to-end analytics project while learning SQL and Power BI.  
I focused on understanding data modeling, ETL using SQL, and building meaningful business dashboards.

The goal of the project is to showcase **data modeling, SQL transformations, and business analytics** in a real-world scenario.

---

## 🛠️ Tools & Technologies

- MySQL 8.0  
- SQL (DDL, DML, Joins, Indexing, Aggregations)  
- Power BI  
- CSV files (Global Superstore dataset)

---

## 🗂️ Data Architecture

The database follows a **star schema design**.

### Fact Table
- `orders_fact`  
  - sales  
  - profit  
  - quantity  
  - discount  
  - customer_key  
  - product_key  
  - people_key  

### Dimension Tables
- `customers_dim`
- `products_dim`
- `people_dim`

### Staging Tables (ETL only)
- `orders_staging`
- `people_staging`

Staging tables were used for raw data loading and transformation and were **not used in Power BI**.

---

## 🔄 Data Processing Flow

1. Imported CSV files into MySQL staging tables  
2. Cleaned and standardized data using SQL  
3. Removed duplicates from dimension tables  
4. Created surrogate keys for dimensions  
5. Built the fact table using foreign key relationships  
6. Added indexes on foreign keys for performance  

---

## 📈 Power BI Dashboard

### Main Dashboard
- Total Sales
- Total Profit
- Profit Margin
- Total Orders
- Average Order Value
- Average Discount
- Sales Trend by Year
- Sales by Category
- Top 10 Products by Sales
- Interactive slicers (Date, Region, Category, Segment)

### Drill-Through Page
- Product-level performance
- Sales trend for selected product
- Regional sales distribution

---

## ✅ Key Learnings

- Star schema data modeling
- SQL-based ETL process
- Handling drill-through and filter context in Power BI
- Creating business-focused dashboards

---
## ⚠️ Challenges Faced

- Handling duplicate customers while building dimension tables  
- Managing foreign key constraints during fact table reloads  
- Understanding filter context and drill-through behavior in Power BI  
- Fixing NULL values caused by incorrect joins  

These challenges helped me strengthen my understanding of SQL and data modeling.

---

## 📌 Author

**Siddhesh Ganbavale**  
MBA (Finance & Operations)  
Aspiring Data Analyst actively building hands-on projects in SQL and BI tools.  
Skills: SQL | Power BI | Tableau | Python
