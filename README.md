# Ecommerce-Sales-Analysis
“Power BI dashboard for analyzing e-commerce sales and customer trends”

# 📊 E-Commerce Sales Analysis Dashboard (Power BI)
## 📌 Project Overview

This project focuses on analyzing e-commerce sales data from 2021 to 2025 to uncover business insights related to revenue, profitability, customer behavior, and regional performance. An interactive Power BI dashboard was developed to enable dynamic exploration of data and support data-driven decision-making.

---

## 🎯 Business Objective

The primary goal of this project is to:

* Monitor overall business performance through key metrics
* Identify top-performing products and categories
* Analyze sales and profit trends over time
* Understand regional sales distribution
* Provide actionable insights for improving revenue and profitability

---

## 📂 Dataset Description

The dataset consists of structured transactional data, including:

* Order ID, Order Date
* Product Category and Sub-Category
* Sales and Profit values
* Customer details
* Region and location data

The dataset spans multiple years, allowing trend and time-series analysis.

---

## 🧹 Data Cleaning & Transformation

Data preprocessing was performed using Power Query Editor to ensure accuracy and usability:

* Removed duplicate records to maintain data integrity
* Handled null/missing values using replacement and filtering techniques
* Changed data types for consistency (dates, numeric fields)
* Renamed columns for better readability
* Applied transformations like filtering, sorting, and formatting

---

## 📊 Data Modeling

* Established relationships between tables (where applicable)
* Created a structured data model for efficient querying
* Implemented calculated columns and measures using DAX

---

## 📐 DAX Calculations Used

The following DAX functions were used to create meaningful metrics:

* **Total Sales**

  ```DAX
  Total Sales = SUM(Sales[Sales])
  ```

* **Total Profit**

  ```DAX
  Total Profit = SUM(Sales[Profit])
  ```

* **Total Orders**

  ```DAX
  Order Count = COUNT(Sales[Order ID])
  ```

* **Profit Margin**

  ```DAX
  Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
  ```

* **Year-to-Date (YTD) Sales**

  ```DAX
  YTD Sales = TOTALYTD([Total Sales], Sales[Order Date])
  ```

* **Previous Year Sales**

  ```DAX
  Previous Year Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Sales[Order Date]))
  ```

* **Growth Percentage**

  ```DAX
  Sales Growth % = 
  DIVIDE([Total Sales] - [Previous Year Sales], [Previous Year Sales], 0)
  ```

These calculations enabled deeper analysis of trends and performance.

---

## 📈 Dashboard Features

The Power BI dashboard includes the following components:

* **KPI Cards**

  * Total Sales
  * Total Profit
  * Order Count
  * Profit Margin

* **Sales Trend Analysis**

  * Line charts showing sales over time

* **Category & Product Analysis**

  * Bar charts comparing product categories and sub-categories

* **Regional Analysis**

  * Map/visual showing sales distribution by region

* **Interactive Filters (Slicers)**

  * Region
  * Category
  * Date

* **Drill-through Functionality**

  * Enables detailed analysis for specific segments

---

## 🔍 Key Insights

* Certain product categories significantly contribute to total revenue
* Sales show seasonal trends across different years
* Some regions consistently outperform others in terms of sales and profit
* Profit margins vary across categories, highlighting optimization opportunities

---

## 💼 Business Impact

This dashboard helps stakeholders to:

* Track and monitor business performance in real-time
* Identify high-performing and underperforming areas
* Make strategic decisions based on data insights
* Improve operational efficiency and profitability

---

## 📁 Project Files Included

* 📄 Ecommerce Sales Report (PDF)
* 📊 Presentation Slides (PPT)
* 📂 Dataset (Excel)
* 📈 Power BI Dashboard (.pbix)
* 🖼️ Dashboard Screenshots (PDF/Image)

---

## 👨‍💻 Roles & Responsibilities

* Collected and understood business requirements
* Cleaned and transformed raw data using Power Query
* Designed data model and relationships
* Created DAX measures for KPIs and analysis
* Built interactive and user-friendly dashboard
* Generated insights and documented findings

---

## 🚀 Conclusion

This project demonstrates end-to-end data analysis, from data cleaning to visualization, using Power BI. It highlights the ability to transform raw data into meaningful insights that support business growth and decision-making.


---

