# Inventory Tracking Dashboard
Create a Power BI Dashboard to monitor inventory levels of a bike manufacturer - AdventureWorks
## :one: Project Overview:
**:round_pushpin: The purposes of this project are:**
- Analyse the inventory performance and inventory statsus by product cateogory and factory location between 2011 and 2014
- Suggest inventory control strategies and sales & marketing strategies 
## :two: Dataset Description:
- **Company:** AdventureWorks (fictional)
- **Time period:** from 2011 to 2024
- **Dataset:**
  + Location: LocationID, CostRate, Availability,..
  + Category: Name, ProductCategoryID
  + SubCategory: Name, ProductSubcategoryID
  + Product: ProductID, Attributes (Size, ProductLine, Weight, Style), Reorder Point, SafetyStock Level,..
  + Product Inventory: ProductID, LocationID, Quantity (only snapshot at a certain time, not historical data)
  + Sales Orders: SalesOrderID, OrderDate, ShipDate, DueDate, OrderQty, UnitPrice,...
  + Purchase Orders: PurchaseOrderID, OrderDate, ShipDate, DueDate, ReceivedQty, UnitPrice,...
  + Work Orders: WorkOrderID, StartDate, ShipDate, EndDate, OrderQty, ScrappedQty,...
- **North-star metrics:** Inventory Quantity and Inventory Value
- **Data Modelling:**
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165147.png?raw=true)

## :three: Tools used:
- Power BI (Power Query, DAX measures, Visuals)
## :four: Dashboard Structure:
- **Overview:** Inventory Quantity and Inventory Value by Location, Category, and Product Characteristics + Detailed Table (Number of In stock/Out of Stock/Below Reorder Point/Below Safety Level Products) <br>
- **Analysis:** Order Quantity, Manufactured Quantiy, Purchased Quantity over time + detailed information by Category (Inventory Qty/Revenue/Sales Qty/Profit Margin) <br>
- **Lead Time:** Lead Time and Lead Time Delays over time and by Category  <br>
- **Insights:** Inventory Control Strategies + Sales & Marketing Strategies
## :five: Dashboard: [attached file]()
### :one: Overview: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165712.png?raw=true)
- Total Inventory Value: ~$20M — a high-value stock, so optimization is crucial.
#### 📌 By location:
+ Subassembly, Miscellaneous Storage, and Tool Crib together hold over 75% of total stock —> which may indicate space utilization issues or process inefficiencies.
#### 📌 By Category:
+ A huge portion of inventory is under "No Data" — suggesting missing categorization or poor data hygiene
+ Bikes and Components had the highest inventory quantity (~47K and ~15K respectively) since they are core products 
#### 📌Inventory Health: 
+ Below Reorder Point: 272 items (54% of products).
+ Below Safety Stock Level: 376 items — that's ~75% of products, which implies a serious risk of stockouts.
+ Out-of-Stock Rates were 15.08% on average, and the highest in 'Frames' SubCategory (all above 75%)
+ Reorder Efficiency were 46.03% on average, and the lowest in 'Frames' SubCategory (all below 25%)
### :two: Analysis: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165248.png?raw=true)
#### 📌 Sales & Profit Margin Trend:
+ Sales Quantity grew consistently from 2011 to mid-2013 and peaked in Q3 2013. After Q3 2013, sales quantity began to decline, possibly due to overstocking, seasonality, or decreased demand.
* By Sales:
  + Bikes and Accessories led in sales
  + Bikes had the highest volume.
  + Accessories showed strong and consistent growth too.
* By Profit Margin:
  + Accessories had the highest profit margin, at 50% on average, followed by Clothing (14.6%)
  + The figures for Bikes experienced a significant decline in 2012, however, they recovered strongly after Q2/2013
  + The figures for Components showed a steady increase, but still remained low (4.2% on average)
#### 📌 Manufacturing Trend:
+ Sharp increase in manufactured quantity (Bikes) from 2011 to 2013.
+ The decline in manufacturing after Q3 2013 aligns with the drop in sales — suggesting production matched demand, or production capacity reached a limit.
+ Bikes are core manufactured products, not purchased externally.
#### 📌 Purchasing Trend:
+ Purchasing quantity spiked post-2012, especially in Components and Accessories --> Indicates increased reliance on external suppliers to meet demand as internal manufacturing focused on Bikes.
+ Sales quantity increased dramatically after Q2/2024, aligning the patterns of Purchasing Trend --> Suggesting purchasing matched demand
+ By Category:
  + Components hold the most inventory but have low profit margin (4.2%).
  + Accessories have the highest profit margin (50%) with moderate inventory levels.
  + Bikes, although sold the most, have low margin (8.4%) → possible focus on volume over profitability.
+ By SubCategory:
  + Top-performing Categories (High Sales & High Margin): Bikes (Mountain Bikes) & Accessories (Helmets, Tire & Tubes)
  + Problematic Categories (High Sales & Low Margin): Components (Mountain/Road/Touring Frames) & Clothing (Jerseys & Caps)

### :three: Lead Time: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165352.png?raw=true)
#### 📌 Trends over time:
+ Fulfillment and Procurement Lead Time are relatively stable (at 7 and 9 days respectively), while Production Lead Times slightly increased, varying around 12-14 days.
+ Production Lead Time Delay is consistently > 0, while fulfillment/procurement delays remain mostly negative, indicating:
  + Fulfillment/Procurement always complete early (5 days earlier on average)
  + Production is consistently behind schedule (4.6 days for bikes and 2.8 days for components) 
+ Delayed WorkOrder Rates:
  + Nearly 1 in 3 Work Orders are delayed, indicating a critical area for improvement in manufacturing scheduling or execution.
  + Bikes had the alarmingly highest delayed rates (55.95%), followed by Components (36.28%)
#### 📌 By Category:
+ Clothing has the highest Procurement Lead Time (25 days)
+ In terms of Production Lead Time, Bikes were the highest (16 days), followed by Components (14 days)
### :four: Insights: <br>
#### 📌 Inventory Control Strategies:
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165438.png?raw=true)
#### 📌 Sales & Marketing Strategies:
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165514.png?raw=true)







