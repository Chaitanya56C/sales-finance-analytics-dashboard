# Superstore Sales Dashboard – Power BI

This project is a part of my *Data Analyst Internship Task*.  
I built an interactive dashboard using *Power BI* to analyze Superstore sales performance, profitability, and customer trends.

## Deliverables
- 'pbix/Superstore_Dashboard.pbix' — Power BI report file  
- 'ppt/Superstore_Dashboard_Summary.pptx' — PPT summary with insights & recommendations  
- 'screenshots/' — key screenshots for README preview  
- 'data/Superstore.xlsx' — dataset

## Key Features
- Trend analysis: Sales and Profit over time (Date table used)
- Sub Category-wise and region-wise sales insights
- Sales and profit trend analysis 
- Sub Category performance charts  
- Shape Map — Sales by State/City  
- ShipMode / Market analysis  
- Interactive slicers: Year, Category, Market
  
## Dashboard Components

### Summary KPI Cards
- *Total Sales*  
- *Total Profit*  
- *Total Orders*
- *Profit margin %*

### Visual Charts
- Stacked Chart: Total Sales by Sub.Category and Segment 
- Line Chart: Total Sales by Date    
- Bar Chart: Total Shipping Cost by Ship Mode
- Shape Map: Total Sales by State and Region  

### Table (Created in Dashboard)
A detailed table was created in the dashboard to display key fields:

- *Order ID*  
- *Product Name*  
- *Sum of Sales*  
- *Sum of Profit*  
- *Ship Date*

This table helps in reviewing transaction-level insights and validating summary metrics.

## Measures (DAX)

Total Sales = SUM( Superstore[Sales] )
Total Profit = SUM( Superstore[Profit] )
Total Orders = DISTINCTCOUNT( Superstore[Order ID] )
Profit Margin % = DIVIDE( [Total Profit], [Total Sales], 0 )
Avg Order Value = DIVIDE( [Total Sales], [Total Orders], 0 )
Total Shipping Cost = SUM( Superstore[Shipping Cost] )

## Tools Used
- *Power BI*
- *Excel / CSV Dataset*
- *Data Cleaning & Transformation (Power Query)*

## Insights Discovered
- Technology category contributes the highest revenue  
- Certain sub-categories show negative profit margins  
- December shows a peak in order volume  
- Standard Class is the most used shipping mode  


  
