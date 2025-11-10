# Sales Performance Analysis

This project analyzes sales performance data for a retail store to uncover trends, key profit drivers, and actionable insights.

## Tools Used
- Excel / Power BI

## Skills Demonstrated
- Data Cleaning
- KPI Analysis
- Dashboard Creation
- Insight Reporting

## Data Cleaning Process

The raw dataset was provided in CSV format and was cleaned in Microsoft Excel to prepare it for analysis. The following steps were carried out:

1. **Converted CSV to Excel Workbook:**  
   Saved the file as an `.xlsx` workbook to enable full use of Excel features.

2. **Removed Duplicates:**  
   Used *Data → Remove Duplicates* on the entire dataset to eliminate repeated records.

3. **Checked for Missing Values:**  
   Used *Go To Special → Blanks* to identify empty cells.  
   Rows with missing critical fields such as `Order ID`, `Order Date`, `Sales`, or `Profit` were removed.

4. **Verified and Corrected Data Types:**  
   - `Order Date` and `Ship Date` were formatted as **Date**.  
   - `Sales`, `Profit`, and `Discount` were formatted as **Number**.  
   - `Quantity` was formatted as **Number (no decimals)**.  
   - All categorical fields (e.g., `Region`, `Category`, `Product Name`) were formatted as **Text**.

5. **Added Profit Margin Column:**  
   Created a new calculated field named **Profit Margin (%)** using the formula:  
   `=IF(Sales<>0, Profit/Sales, 0)`  
   Formatted as **Percentage**.

6. **Checked for Outliers:**  
   Sorted `Sales` and `Profit` fields to detect unusual values.  
   Outliers were retained to preserve the completeness and realism of the business dataset.

The cleaned dataset was then saved as `Superstore_Sales_Cleaned.xlsx` for further analysis.

## Exploratory Data Analysis (EDA)

Exploratory analysis was conducted using PivotTables and PivotCharts in Microsoft Excel to identify key sales and performance patterns. The following analyses were performed:

### 1. Sales and Profit by Region
A PivotTable was created with **Region** as the row field and **Sales** and **Profit** as value fields.  
This provided insight into:
- Overall revenue contribution by region  
- Regional profitability  
- Identification of high- and low-performing areas

### 2. Sales by Category and Sub-Category
A PivotTable was created with **Category** and **Sub-Category** as row fields and **Sales**, **Quantity**, and **Profit** as value fields.  
This analysis identified:
- The most profitable product categories  
- Sub-categories contributing the highest revenue  
- Low-performing or unprofitable product lines

### 3. Monthly Sales Trend
A PivotTable was created with **Order Date** grouped by **Month** and **Year**, with **Sales** as the value field.  
A PivotChart (line chart) was added to visualize:
- Monthly seasonality  
- Sales growth or decline trends  
- Peak and low-performing months

### 4. Top 10 Products by Sales
A PivotTable was created with **Product Name** as the row field and **Sales** as the value field.  
A Top-10 filter was applied to identify:
- Best-selling products  
- Product types driving the highest revenue  
