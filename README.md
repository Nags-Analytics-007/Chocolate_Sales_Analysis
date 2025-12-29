# Chocolate Sales Analysis – Power BI Dashboard

## Project Overview
This project is an interactive Power BI dashboard that analyzes chocolate sales performance for a fictitious retail business.  
The goal is to help stakeholders quickly understand total sales, shipment volume, profitability, and top‑performing products and salespersons over time.

## Data Source
- Example sales data provided in Excel format.
- Key fields include: date, region/country, product, boxes sold, sales amount, shipment count, and cost.
- Data was loaded into Power BI and modeled to support flexible slicing and filtering.

## Data Preparation
- Cleaned the raw Excel data by:
  - Handling missing values and correcting data types.
  - Removing inconsistencies and ensuring referential integrity between tables.
- Built a dedicated calendar table and created relationships to the fact table in the model view for proper time‑intelligence calculations.
- Defined a star‑schema style model to keep filters and interactions intuitive across visuals.

## DAX Measures & KPIs
Created multiple DAX measures to support analysis and filtering, including but not limited to:
- **Total Amount** – overall sales revenue.
- **Total Boxes** – total quantity sold in boxes.
- **Shipment Count** – total number of shipments.
- **Total Profit** – revenue minus cost.
- **Profit %** – profitability ratio used across visuals.
- Year‑over‑year comparisons such as **Amount CY vs PY** and **Boxes CY vs PY** to compare current year performance with prior year.

These measures power the cards at the top of the dashboard and the detailed visuals throughout the page.

## Dashboard Layout & Interactivity
The dashboard consists of a single, highly interactive page with multiple tiles:
- **Summary cards** for Total Amount, Total Boxes, Shipment Count, Total Profit, and Profit %, giving a quick performance snapshot.
- **Line charts** for *Amount CY vs PY* and *Boxes CY vs PY* to track sales and volume trends over time.
- **Histogram / distribution chart** for *Shipment Distribution* to understand how shipment counts are spread.
- **Donut chart** for *Amount by Geo* to compare sales contribution by country/region.
- **Top Sales Persons table** showing total boxes, total amount, and profit % for each salesperson.
- **Top 6 Products tile** and **Our Products table** listing products with Total Amount and Profit %, highlighting best and worst performers.

All visuals are connected through the underlying data model:
- Slicers (including a date range slider) allow users to filter the entire dashboard by time period.
- Selecting a region, product, or salesperson filters other visuals, enabling drill‑down into specific segments.

## Key Insights
- Quickly identify the most profitable products and those with negative or low profit margin.
- See which countries/regions contribute the most to total sales and profit.
- Monitor sales and shipment trends over time and compare current year performance against the previous year.
- Recognize top‑performing salespersons based on volume, revenue, and profit %.

## How to Use This Dashboard
1. Download the `Chocolates_Sales_Analysis.pbit` file from this repository.
2. Open it in Power BI Desktop (latest version recommended).
3. Provide the required data source path/parameters if prompted, and refresh the data.
4. Use the date slider, product filters, and other slicers to interact with the visuals and explore the chocolate sales performance from different perspectives.
