# Data-warehouse
Data Warehouse Implementation for Sales and Inventory Management
# Introduction 
In today’s dynamic business environment, retail and distribution sectors face constant 
challenges in managing inventory efficiently while driving sales growth. Data is abundant, but 
its fragmentation across multiple systems makes it difficult to gain meaningful insights. 
Businesses often struggle with balancing inventory levels, identifying high-performing 
products, and understanding customer preferences. To address these challenges, a centralized 
solution is needed to streamline data management and enable better decision-making. 
This project aims to design and implement a Sales and Inventory Management Data 
Warehouse, providing a single platform to consolidate and analyze data from multiple 
dimensions. By leveraging advanced analytical techniques, the system will empower 
stakeholders to explore sales trends, optimize inventory management, and evaluate supplier 
and customer performance effectively. The goal is to transform raw data into actionable 
insights, enhancing operational efficiency and profitability.
# 📦 ISM6208 Final Project – Data Warehousing

## 🚀 Project Title
**A Comprehensive Data Warehouse Implementation for Sales and Inventory Management**

## 👨‍🎓 Course Info
- **Course**: ISM 6208 – Data Warehousing
- **Instructor**: Prof. Han Reichgelt
- **Institution**: University of South Florida
- **Team**: Group 10  
  👤 Ruchitha Paccha (U70955896)  
  👤 [Add other team members here]

---

## 📘 Project Overview

In today’s fast-paced retail environment, managing inventory and sales data efficiently is crucial for maintaining competitive advantage. However, data silos and scattered systems hinder effective analysis. This project provides a unified **data warehouse** platform that consolidates sales, inventory, customer, product, and supplier data for a retail enterprise.

Our star schema design and OLAP-powered queries enable businesses to extract insights quickly, support decision-making, and optimize inventory and sales operations.
## 🧱 Star Schema Design

### 🎯 Fact Table: `DW110.SALES`
Captures transactional data with key metrics:
- `QUANTITY_SOLD`
- `TOTAL_REVENUE`
- `SALES_CHANNEL`

### 🧩 Dimension Tables
- `DW110.PRODUCT` – Product details and pricing
- `DW110.CATEGORY` – Product category descriptions
- `DW110.SUPPLIER` – Supplier info and ratings
- `DW110.CUSTOMER` – Customer segments and contacts
- `DW110.LOCATION_DIMENSION` – Geographical breakdown
- `DW110.TIME_DIMENSION` – Date, Month, Quarter, Year hierarchy
- `DW110.INVENTORY` – Inventory levels, restock history
- `DW110.WAREHOUSE` – Warehouse locations and capacity

Visual ER diagram available in `/visuals/ERD.png`.
![image](https://github.com/user-attachments/assets/275d99f5-e00c-4465-a113-b41b7cb9f6e5)


## 🧠 Key Functionalities
### 🔍 OLAP Operations Implemented
- **Aggregation**: Revenue & quantity sold by product, region, category
- **Drill-Down**: From category → product → supplier
- **Roll-Up**: Weekly → Monthly → Quarterly sales trends
- **Ranking**: Top N customers by revenue
- **Window Functions**: `LAG`, `LEAD` for time-series revenue and stock analysis
- **Moving Averages**: Smoothing sales data over months

### 📊 Data Visualizations
Charts are stored in `/visualizations/`:
1. **Line Chart**: Monthly revenue trends
2. **Bar Chart**: Product stock vs reorder levels
3. **Scatter Plot**: Customer purchasing behavior
4. **Pie Chart**: Sales distribution by channel
5. **Heatmap**: Correlation matrix of KPIs

  

