# Simple Sales Dashboard Design

## Project Overview
This project demonstrates the creation of a **basic interactive sales dashboard** using Power BI (or Tableau) to visualize sales performance by product, region, and month. The dashboard allows users to explore trends, compare regions, and analyze category contributions through interactive visuals.

## Tools Used
- **Power BI Desktop** 

## Dataset
The dataset used is `Superstore_Sales.csv` with the following columns:
- `Order Date` – Date of the order  
- `Region` – Sales region  
- `Category` – Product category  
- `Sales` – Sales amount  
- `Profit` – Profit amount  

## Steps to Create the Dashboard

1. **Import Dataset**
   - Load the CSV file into Power BI or Tableau.  
   - Check column names and data types.  

2. **Data Preparation**
   - Convert `Order Date` to **Date type**.  
   - Create a new **Month-Year** column for time-based analysis:
     ```DAX
     MonthYear = FORMAT([Order Date], "MMM-YYYY")
     ```

3. **Create Visuals**
   - **Line Chart:** `Monthly Sales Trend` (X-axis: Month-Year, Y-axis: Sales)  
   - **Bar Chart:** `Sales by Region` (X-axis: Region, Y-axis: Sales)  
   - **Donut Chart:** `Sales Distribution by Category` (Values: Sales, Legend: Category)  

4. **Add Interactivity**
   - Insert a **Slicer** for `Region` or `Category` to filter visuals dynamically.  
   - Enable cross-filtering between charts.  

5. **Formatting & Colors**
   - Highlight top-performing regions or categories with distinct colors.  
   - Ensure all visuals have readable titles, labels, and consistent color themes.  

6. **Export Dashboard**
   - Save the dashboard as a **PDF** or take a **screenshot** for deliverables.
