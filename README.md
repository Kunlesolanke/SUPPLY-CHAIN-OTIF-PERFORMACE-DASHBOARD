# SUPPLY-CHAIN-OTIF-PERFORMACE-DASHBOARD
An interactive Power BI dashboard built to monitor order fulfillment performance across regions, warehouses, and transport modes with a focus on On-Time-In-Full (OTIF) delivery tracking.

## DATA SET USED
https://drive.google.com/drive/mobile/folders/1aZmwnuDuCCF4nRbwwcQXRyQXhBvNlnIK?usp=sharing

## 🧩 Business Problem
A distribution company operating out of a Bangalore warehouse was struggling to understand why customer complaints about late or incomplete deliveries kept rising, despite orders leaving the warehouse on schedule. Management had no unified view of:
1.Which regions were consistently missing delivery targets
2.Whether delays were caused by which transport mode (Ship, Truck, or Air) was used
3.How On-Time (OT), In-Full (IF), and combined On-Time-In-Full (OTIF) rates compared across the business
4.The gap between ordered quantity vs. delivered quantity per shipment.

Without this visibility, the business couldn't pinpoint whether the issue was a specific region, a specific carrier, or a warehouse-level bottleneck making it impossible to fix efficiently.

## 🛠️ Steps Taken
1.Data preparation Cleaned and structured raw order-level data (order dates, promised delivery dates, actual delivery dates, ordered qty, delivered qty, region, warehouse, transport mode) in Power Query.
2.Data modeling — Built relationships between orders, region, and transport mode tables to support cross-filtering.
3.DAX measures — Created core KPIs:
4.OT %  = % of orders delivered on or before the promised date
5.IF % = % of orders delivered with the full ordered quantity
6.OTIF % = % of orders that were both on-time and in-full
7.Average Delay = average number of days late, by warehouse and by transport mode
8.Visualization — Designed a single-page dashboard with:
9.KPI cards (Total Orders, OT%, IF%, OTIF%)
10.OTIF% by Region (bar chart)
11.IF% and OT% by Region (comparison bar chart)
12.Combined trend of OTIF%, IF%, OT% by Region (line chart)
13.Average delay by Warehouse Location
14.Average delay by Transport Mode (donut chart)
15.Ordered Qty vs Delivered Qty (bar chart)
Interactivity — Added slicers for Warehouse Location, Transport Mode, Region, and Month/Year so stakeholders can drill into any segment.
Customization — Adapted the layout and metric selection from the original tutorial reference to better fit a warehouse-level OTIF reporting use case, including the added Average Delay by Transport Mode breakdown.
