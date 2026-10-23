# Retail Store Sales Analysis and Visualization

## Project overview
This FDVA mini project demonstrates retail transaction analysis using Python, Power BI, and Tableau. The supplied dataset contains 200 sample transactions. It is synthetic practice data, not real business records.

## Files
- `Retail_Store_Sales_Mini_Project.pdf` — formatted mini-project report.
- `Retail_Store_Sales_Mini_Project.docx` — editable report source.
- `Retail_Sales_Data.csv` — raw sample dataset.
- `Cleaned_Retail_Sales.csv` — cleaned dataset for visualisation and dashboard tools.
- `retail_sales_analysis.py` — reproducible Python cleaning and chart-generation script.
- `README.md` — project setup and usage guide.

## Requirements
Python 3.10 or newer; packages: `pandas`, `numpy`, `matplotlib`, and `seaborn`.

Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```

## Run the analysis
Place the raw CSV and Python script in the same folder, then run:
```bash
python retail_sales_analysis.py
```
The script loads the raw dataset, fills missing values, standardises date and numeric fields, recalculates derived metrics, exports `Cleaned_Retail_Sales.csv`, and saves eight chart images.

## Power BI
1. Open Power BI Desktop.
2. Select **Get data → Text/CSV** and import `Cleaned_Retail_Sales.csv`.
3. Create KPI cards for Net Sales, transaction count, average discount and average customer rating.
4. Add charts for category-wise transactions, net sales by city, sales by month and sales by channel.
5. Add slicers for City, Product Category, Sales Channel and Payment Method.
6. Check date sorting and currency formatting before publishing.

## Tableau
1. Open Tableau Desktop/Public and connect to `Cleaned_Retail_Sales.csv`.
2. Create worksheets for monthly net sales, category sales, sales channel share, city-wise sales and average customer rating.
3. Assemble the worksheets into a dashboard.
4. Add filters for City, Product Category, Sales Channel, Payment Method and Year.

## Data dictionary (selected fields)
- `Transaction_ID`: unique transaction identifier.
- `Sale_Date`: transaction date.
- `City`, `Store_ID`: store location fields.
- `Product_Category`, `Product_Name`: product classification.
- `Units_Sold`, `Unit_Price_INR`: quantity and unit price.
- `Gross_Sales_INR`: units sold multiplied by unit price.
- `Discount_INR`: discount amount.
- `Net_Sales_INR`: gross sales minus discount.
- `Sales_Channel`, `Payment_Method`: transaction channel and payment type.
- `Customer_Rating`: customer rating from 2 to 5 in the generated sample.
- `Discount_Percentage`: discount as a percentage of gross sales.

## Important note
The dashboard pictures in the report are illustrative layout mockups, not screenshots of live Power BI or Tableau reports. The data and results are generated for educational demonstration. Build the dashboards in the respective applications to obtain working interactive filters.
