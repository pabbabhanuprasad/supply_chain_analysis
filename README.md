#  Supply Chain Analytics Project (LogiScale BigData)

## Project Overview
This project focuses on analyzing global supply chain and logistics data to identify delivery delays, optimize routes, and improve operational efficiency.  
The system processes large-scale shipment data using PySpark and visualizes insights using Power BI dashboards.


## Objectives
- Analyze delivery delays across regions and carriers
- Identify factors affecting shipment performance
- Optimize supply chain operations using data-driven insights
- Build interactive dashboards for business users

## Architecture
1. Data Ingestion (CSV / Raw Files)
2. Data Processing using PySpark
3. Data Modeling (Star Schema)
4. Data Visualization (Power BI)

---

## Data Model (Star Schema)

### Fact Table:
- `fact_logistics`
  - shipment_id
  - shipment_date
  - warehouse_id
  - sku_id
  - delay_hours
  - delay_status
  - source_city
  - destination_city
  - route_id
  - inventory_level
  - gps_id
  - latitude
  - longitude
  - speed_kmph
  - timestramp
  - record_type
    

### Dimension Tables:
- `dim_product`
- `dim_warehouse`
- `dim_date`


## ⚙️ Technologies Used
- PySpark (Data Processing)
- SQL (Data Analysis)
- Power BI (Dashboard)


## Data Processing Steps
- Data Cleaning (Handling null values, duplicates)
- Feature Engineering (Delay calculation)
- Data Transformation
- Aggregations for KPIs
-Dashboards created by Power BI



## 📊 Key KPIs
- Average Delivery Delay
- On-Time Delivery %
- Total Shipment Cost
- Region-wise Performance
- Carrier Performance

## Dashboards
### 1. Logistics Shipments Performance Dashboard
- Delay trends
- On-time delivery %
- Total Shipment by Destination City
- Total Shipment by Delivery Status
- Total Shipment by Warehouse_id
- Avg Delay By Route_id

### 2. GPS tracking & Speed Analytics Dashboard
- Total GPS records
- Speed Distribution
- Top Shipments by Speed
- Avg Delay by Route_id
- Avg Speed trends

### 3. Inventory Optimization & Warehouse Stock Monitoring Dashboard
- Total Inventories
- Lowest SKU_ID
- Total Inventory by Month
- Total Inventory by Warehouse_id
- Total Inventory by sku_id
- Low Stock Analysis
