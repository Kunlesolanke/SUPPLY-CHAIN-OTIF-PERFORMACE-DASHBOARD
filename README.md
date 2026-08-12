# SUPPLY-CHAIN-OTIF-PERFORMACE-DASHBOARD
An interactive Power BI dashboard built to monitor order fulfillment performance across regions, warehouses, and transport modes with a focus on On-Time-In-Full (OTIF) delivery tracking.

## DATA SET USED
https://drive.google.com/drive/mobile/folders/1aZmwnuDuCCF4nRbwwcQXRyQXhBvNlnIK?usp=sharing

## 🧩 Business Problem
A distribution company operating out of a Bangalore warehouse was struggling to understand why customer complaints about late or incomplete deliveries kept rising, despite orders leaving the warehouse on schedule. Management had no unified view of:
1. Which regions were consistently missing delivery targets

2. Whether delays were caused by which transport mode (Ship, Truck, or Air) was used

3. How On-Time (OT), In-Full (IF), and combined On-Time-In-Full (OTIF) rates compared across the business

4. The gap between ordered quantity vs. delivered quantity per shipment.

Without this visibility, the business couldn't pinpoint whether the issue was a specific region, a specific carrier, or a warehouse-level bottleneck making it impossible to fix efficiently.

## 🛠️ Steps Taken
1. Data preparation: I Cleaned and structured raw order-level data (order dates, promised delivery dates, actual delivery dates, ordered qty, delivered qty, region, warehouse, transport mode) in Power Query.

2. Data modeling : Built relationships between orders, region, and transport mode tables to support cross-filtering.

3. DAX measures  Created core KPIs:

* OT %  = % of orders delivered on or before the promised date

* IF % = % of orders delivered with the full ordered quantity

* OTIF % = % of orders that were both on-time and in-full

* Average Delay = average number of days late, by warehouse and by transport mode

4. Visualization — Designed a single-page dashboard with:

* KPI cards (Total Orders, OT%, IF%, OTIF%)

*  OTIF% by Region (bar chart)

* IF% and OT% by Region (comparison bar chart)

* Combined trend of OTIF%, IF%, OT% by Region (line chart)

* Average delay by Warehouse Location

* Average delay by Transport Mode (donut chart)

* Ordered Qty vs Delivered Qty (bar chart)

5. Interactivity : Added slicers for Warehouse Location, Transport Mode, Region, and Month/Year so stakeholders can drill into any segment.

6. Customization:  Adapted the layout and metric selection from the original tutorial reference to better fit a warehouse-level OTIF reporting use case, including the added Average Delay by Transport Mode breakdown.

## LINK TO FULL PROJECT 
https://1drv.ms/b/c/B35DBD2D8A213BFB/IQC_m1BLPUFWQYIs9XRtQA3IAQCL3xh6u2IPRafB9CsqijM?e=4UwQhk

## dashboard interaction
https://1drv.ms/u/c/B35DBD2D8A213BFB/IQBfOXBPA_1CSJeKv7zSQzg3AWWcfj25h4cFY9b64xHG0FU?e=ROtBnm

 
## Key Insights

1. The company has 15 orders.

2. 73.33% of the orders arrived on time.

3. Only 53.33% of orders were delivered completely.
This is the biggest concern. It means many customers received their orders, but some items or quantities were missing.

4. Overall OTIF is 66.67%.
OTIF means the order was delivered on time AND with the complete quantity.
So, only about 2 out of every 3 orders met both requirements.

5. The West region is performing the worst.
Its OTIF is 0%, meaning none of the orders there met both the on-time and complete-delivery requirements.

6. The North region also needs improvement.
Its OTIF is 50%, meaning only half of the orders met the requirement.

7. East and South are performing better.
  
8. Both have 100% OTIF, so they are currently the best-performing regions.

* The main thing the business should investigate

* The biggest problem doesn't seem to be only late deliveries. The bigger issue is that orders are not always being delivered completely.

* So the company should check:

  Are products out of stock?

  Are suppliers providing the correct quantities?

  Are warehouses picking the correct items?

  Which products are frequently missing?

  Why is the West region performing poorly?

* In one sentence to my  client:

"The dashboard shows that while most orders are arriving on time, many are not being delivered completely. The West and North regions need the most attention, while East and South are performing well. The business should focus on improving inventory and order fulfillment to increase the overall OTIF rate."

## DASHBOARD IMAGE 
<img width="1920" height="1080" alt="DASH BOARD SCREENSHOT" src="https://github.com/user-attachments/assets/66b49793-b66e-4e4a-98ad-cc97d82ede8a" />

## RECOMMENDATIONS
The company should prioritize improving order completeness and investigate the poor performance in the West and North regions. Improving inventory management, supplier performance, and warehouse processes should help increase the overall OTIF rate from 66.67% to a higher level.
