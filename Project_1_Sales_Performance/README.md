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
