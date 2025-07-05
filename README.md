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
### :two: Analysis: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165248.png?raw=true)
### :three: Lead Time: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165352.png?raw=true)
### :four: Insights: <br>
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165438.png?raw=true)
![alt](https://github.com/NguyenPhuongNghi/Inventory-Tracking/blob/main/photos/Screenshot%202025-07-05%20165514.png?raw=true)







