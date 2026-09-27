# 🛒 Blinkit Sales & Operations Dashboard --- Power BI

## 📌 Project Overview

An interactive Power BI Sales &amp; Operations Dashboard built to analyze quick-commerce performance across orders, sales, delivery, ratings, cancellations, cities, zones, and product categories.  The project demonstrates practical use of Power Query, DAX, data modeling, KPI cards, slicers, bookmarks, buttons, and interactive visualizations.

## 🖼️ Dashboard Preview
https://github.com/mahakdhyani/Blinkit-Sales-Dashboard/blob/main/Blinkit%20Sales%20Dashboard%20Image.png

## 🎯 Key KPIs
The dashboard currently highlights the following KPIs:
KPI                       Value shown
Total Orders                      999
Total Sales                      220K
Average Order Value            220.08
Average Delivery Time           18.40
Average Ratings                  3.97
Cancellation Rate                  7%
These values are based on the dashboard view shown in the project
screenshot.

## 📌 Dashboard Features

1. Filter Panel
The left-side filter panel allows the report user to filter the
dashboard by:
- City
- Zone
- Category
This makes the report useful for exploring performance across different
operational segments.

2. KPI Cards
The top KPI cards provide an at-a-glance summary of:
- Total Orders
- Total Sales
- Average Order Value
- Average Delivery Time
- Average Ratings
- Cancellation Rate

3. City-Level Net Sales

The Net Sales by City chart compares sales performance across cities
such as:
Jaipur
Chennai
Mumbai
Kolkata
Delhi NCR
Bengaluru
Hyderabad
Pune

4. Order Status Analysis
The Total Orders by Order Status visual separates orders into:
- Delivered
- Cancelled
- Returned
This helps identify the overall distribution of successful and
unsuccessful orders.

5. Monthly/Time-Based Sales Analysis
   
The Net Sales by Month Name visual provides a time-based view of
sales and can be used to identify changes in sales performance across
months.

6. Category Performance
   
The Net Sales by Category chart compares product categories
including:
Grocery & Staples
Pet Supplies
Beauty & Personal Care
Home & Office
Cold Drinks & Juices
Fruits & Vegetables
Dairy & Bread
Munchies
Paan Corner

## 🧰 Tools & Technologies
- Microsoft Power BI Desktop
- Power Query for data preparation
- DAX for calculated measures
- Interactive slicers and filters
- Power BI visuals and custom dashboard navigation
- GitHub for project documentation and portfolio presentation

## Data Preparation

The typical workflow for this dashboard is:

Raw Dataset
    ↓
Power Query
    ↓
Data Cleaning & Transformation
    ↓
Data Model
    ↓
DAX Measures
    ↓
Visualizations
    ↓
Interactive Power BI Dashboard

Data preparation can include:

- Removing duplicate records
- Handling missing values
- Correcting data types
- Creating date/month fields
- Standardizing category and city names
- Creating calculated columns where required
- Building measures for KPIs

## Example DAX Measures

The exact formulas depend on the column names in the source dataset.
Typical measures can follow this structure:

- Total Orders = COUNTROWS(Orders)
- Total Sales = SUM(Orders[Sales])
- Average Order Value =DIVIDE([Total Sales], [Total Orders])
- Average Rating =AVERAGE(Orders[Rating])
- Cancellation Rate =DIVIDE(CALCULATE([Total Orders],Orders[Order Status] = "Cancelled" ),[Total Orders])

Update the table and column names to match the actual dataset.

## 💡 Business Questions Addressed

This dashboard is designed to help answer questions such as:

1. What are the total orders and total sales?
2. What is the average order value?
3. Which cities generate higher net sales?
4. Which categories contribute most to sales?
5. What percentage of orders are cancelled or returned?
6. How does sales performance change over time?
7. What is the average delivery time?
8. What is the average customer rating?
9. How do results change when City, Zone, or Category filters are applied?

## Key Observations From the Shown Dashboard

Based on the displayed dashboard view:

- Total orders are shown as 999.
- Total sales are shown as approximately 220K.
- Average order value is shown as 220.08.
- Average delivery time is shown as 18.40.
- Average rating is shown as 3.97.
- Cancellation rate is shown as 7%.

- Jaipur has the highest displayed city-level net sales in the current view.
- Grocery & Staples is the largest displayed category by net sales.
- The order-status visual shows Delivered orders forming the majority of the displayed order mix.
- These observations describe the current dashboard state and maychange when filters are applied.

## Dashboard Navigation

The left navigation area contains icon-based controls for:

- Home
- Refresh/Retry
- Calendar
- Information

These can be implemented in Power BI using buttons, images/icons, page navigation, and bookmarks.

## 🚀 Portfolio Summary

Blinkit Sales & Operations Dashboard | Power BI

Built an interactive Power BI dashboard to analyze sales, orders,
delivery performance, ratings, cancellations, cities, and product
categories. Implemented KPI cards, interactive filters, time-based
analysis, city/category comparisons, and navigation-style UI elements to
create a clean business intelligence report.
