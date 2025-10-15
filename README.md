# Transportation Data Analytics Project 

## Introduction

This project demonstrates a full data pipeline using:
- **SQL Server** for data storage and management  
- **Excel** for data cleaning and calculations  
- **Power BI** for dashboard visualization 

The dataset covers 6 tables related to vehicle operations:
1. Vehicles  
2. Drivers  
3. Shipments  
4. Deliveries  
5. Fuel_Logs  
6. Maintenance_Records  

## Skill Showcased

### SQL - Data Creation : ###

- All six tables were created in SQL Server Management Studio (SSMS). 
- Each table stores different aspects of transportation data.

### Excel – Data Cleaning & Calculations : ###

- **Data Processing in Excel -** After exporting tables from SQL:
    -  Each table was saved as an individual Excel sheet.
    - Performed necessary cleaning:
    - Removed null values
    - Corrected date formats
    - Checked consistency between tables using `VLOOKUP`
- **Calculations done :** 

    - **Vehicles** - Calculated overall  fuel efficiency and Next service Date & Service Status.
    - **Drivers** - Calculating Trips per Year and Performance of the Driver.
    - **Shipments** - Calculated total shipment cost per km & weight per km.
    - **Deliveries** - Calculating On time Delivery rate and delivery rate (%).
    - **Fuel_Logs** - Calculating Fuel cost per km and average cost from liter.
    - **Maintenance_Records** - Summed the total Maitenance Records.
### Power BI - Dashboard Visualization : ### 

   **Visualization in Power BI -** The cleaned Excel sheets were imported into Power BI.
Relationships were established using `Vehicle_ID` and `Driver_ID`.

#### Transportation Dashboard : ####

![Page 1](/images/Transportation%20dashboard%20page%201.png)

-  Displays overall key performance indicators (KPIs):
   - Average of capacity
   - Sum of Distance
   - Max Rating
   - Average of cost per liter

- **Visuals used :** 
   - Line Chart: Count of deliveries and shipment priorities by month  
   - Scatter Chart: Shipment cost vs. weight vs. delay hours  
   - Stacked Bar Chart: Shipment priority vs. origin  
   - Area Chart: Shipment weight trends by month and priority  
- A **Vehicle_ID slicer** was added for filtering across all visuals.

#### Driver Drill-Through Page : ####

![Page 2](/images/Driver%20Drill%20Through%20page%202.png)

- Focuses on delivery and driver performance.
- KPIs:
  - Total Shipments 
  - Average Rating
  - Total Distance 
- Visuals included:
  - Donut charts for shipment priority and customer feedback  
  - Bar chart for delivery status (Delivered, Pending, Cancelled)
  - Used **drill-through** to allow users to right-click on a driver in the main page and view details on this page.
#### Vehicle Drill-Through Page : ####

![Page 3](/images/Vehicle%20Drill%20Through%20Page%203.png)

- Focuses on vehicle-level performance and cost tracking.
- KPIs:
  - Sum of Distance and Average per Delivery Date  
  - Fuel Efficiency and Distance Target  
  - Maintenance Cost vs. Target
- Visuals included:
  - Treemap showing maintenance cost by workshop and vehicle type  
  - Table showing shipment-wise cost, distance, and weight  
  - Designed **goal tracking visuals** (with target and variance indicators).

## Conclusion ##

Through this project, a complete end-to-end data pipeline was successfully implemented using SQL, Excel, and Power BI.  
The workflow began with structured data creation and management in **SQL Server**, followed by detailed data cleaning and computation in **Excel**, and concluded with insightful visualization in **Power BI**.

This process enabled efficient data handling and meaningful insight generation across six key datasets — Vehicles, Drivers, Shipments, Deliveries, Fuel Logs, and Maintenance Records.

### Key Outcomes:
- Created an integrated dataset connecting vehicles, drivers, and deliveries for real-time analytics.  
- Improved understanding of transportation performance through interactive dashboards and drill-through reports.  
- Identified patterns in cost, delay, and efficiency that can support data-driven decision-making.  
- Demonstrated a practical application of **data integration, transformation, and visualization** using common business tools.

Overall, this project highlights how SQL, Excel, and Power BI can work together to build a **data-driven transportation management system**, improving operational visibility and decision support.