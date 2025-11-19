## 📊 Blinkit Data Analysis – Power BI Dashboard

A complete Business Intelligence project analyzing Blinkit’s sales, customer behavior, and inventory performance using Power BI.
This project helps understand key business metrics like sales trends, outlet performance, item visibility, customer demand, and pricing insights.

## 🚀 Project Overview
- Sales performance across outlets
- Impact of item visibility on sales
- Relationship between fat content and pricing
- Consumer demand patterns
- Outlet establishment trends
- Inventory distribution
The insights are visualized in an interactive Power BI dashboard.

## 🎯 Business Objectives
- Identify top-performing and underperforming outlets.
- Analyze how Item Visibility affects sales.
- Compare the impact of Item Fat Content on revenue.
- Study pricing patterns across product categories.
- Explore outlet-wise distribution of items.
- Provide recommendations to optimize sales & inventory.

## 📂 Dataset Details
- The dataset contains 8,523 records with the following columns:

  | Column Name               | Description                            |
| ------------------------- | -------------------------------------- |
| Item_Identifier           | Unique product ID                      |
| Item_Weight               | Weight of the product                  |
| Item_Fat_Content          | Fat classification (Low Fat / Regular) |
| Item_Visibility           | Shelf visibility percentage            |
| Item_Type                 | Category of the item                   |
| Item_MRP                  | Maximum Retail Price                   |
| Outlet_Identifier         | Unique store ID                        |
| Outlet_Establishment_Year | Store opening year                     |
| Outlet_Size               | Store size description                 |
| Outlet_Location_Type      | Tier 1 / Tier 2 / Tier 3               |
| Outlet_Type               | Supermarket / Grocery                  |
| Item_Outlet_Sales         | Total sales (Target variable)          |

## 📈 Power BI Dashboard Features

✔ Sales Analysis
- Total sales and average sales
- Top 5 & bottom 5 selling items
- Outlet-wise sales comparison

✔ Outlet Insights
- Sales by outlet size (Small / Medium / High)
- Sales by location type (Tier 1 / 2 / 3)
- Store establishment year analysis

✔ Item Insights
- Sales by Item Type
- Distribution of Item MRP
- Fat content vs sales comparison

✔ Visibility & Price Insights
- Relationship between Item Visibility and Sales
- Price segments and their contribution to revenue

✔ Filters / Slicers
- Outlet Type
- Item Type
- Fat Content
- Price Range
- Outlet Location

## 🛠️ Tools & Technologies

| Tool            | Purpose                                                  |
| --------------- | -------------------------------------------------------- |
| **Power BI**    | Data cleaning, modeling, DAX calculations, visualization |
| **Excel / CSV** | Raw data                                                 |
| **Power Query** | Data preprocessing                                       |
| **DAX**         | Measures, calculated columns                             |

## 🧹 Data Cleaning & Preprocessing

Performed in Power Query:
-  Missing value handling
-  Standardizing item fat labels
-  Removing inconsistent visibility values
-  Creating bins for Item MRP
-  Converting data types
-  Creating calculated columns

## 📊 Key DAX Measures Used

Total Sales = SUM('Blinkit'[Item_Outlet_Sales])

Avg Sales = AVERAGE('Blinkit'[Item_Outlet_Sales])

Total Items = COUNT('Blinkit'[Item_Identifier])

Sales by Fat % = 
CALCULATE(SUM('Blinkit'[Item_Outlet_Sales]), Blinkit[Item_Fat_Content])

## ⭐ Insights Summary

- Medium-sized outlets generate the highest total sales.
- Tier 3 locations show stronger revenue compared to Tier 1 and Tier 2.
- Products with Regular Fat Content sell more than Low Fat items.
- Higher Item Visibility does NOT always increase sales — visibility needs strategic positioning.
- Items in the high MRP range contribute the largest revenue share.

## 🧠 Business Recommendations

- Increase product variety & stock in high-performing outlets.
- Improve item placement to increase visibility effectiveness.
- Offer discounts on low-selling MRP ranges.
- Expand more outlets in Tier 3 locations.
- Promote Regular Fat Content products as they perform better.
