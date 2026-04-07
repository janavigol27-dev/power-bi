Sales \& Customer Intelligence Dashboard



Project Overview



The Sales \& Customer Intelligence Dashboard is a comprehensive Power BI project designed to analyze sales performance, customer behavior, and regional trends. This project follows a professional Star Schema data model and provides actionable insights through interactive visualizations and advanced DAX measures.



Key Objectives 



Build a robust data model with a Star Schema layout.



Implement complex DAX formulas for KPIs and measures.



Apply Time Intelligence (YOY, MOM, YTD) to track growth.



Create a multi-page interactive report with enhanced UX/Navigation.



Ensure Mobile Compatibility and Row-Level Security (RLS).



Dataset Description 



The analysis is based on six core tables:



Sales \_Fact: Contains transactional data.



Returns \_Fact: Tracks product returns.



Product \_Dim: Product details and categories.



Customer \_Dim: Customer demographics and segments.



Date \_Dim: Calendar details for time intelligence.



Region \_Dim: Geographical data for regional analysis.



Key Features \& Technical Tasks



1\. Data Modeling



Established relationships between Fact and Dimension tables using Primary \& Foreign Keys.



Designed a clean Star Schema for optimal performance.



2\. DAX Measures \& Calculations



Created core measures using CALCULATE, SUMX, COUNTX, and AVERAGEX.



Developed Time Intelligence measures for:



YOY (Year-Over-Year) Sales Growth.



MOM (Month-Over-Month) Sales Trends.



YTD (Year-To-Date) Total Sales.



Implemented SWITCH logic for KPI classification and RELATED for joining values.



3\. Visualizations \& UI/UX



Main Dashboard: High-level KPIs, Sales/Profit trends by Month, and Segment-wise analysis.



Customer Detail Page: Focuses on Top N Customers and Customer Performance.



Matrix Heatmap: Used advanced conditional formatting to identify sales density across regions and time.



Interactive Slicers: Dynamic filtering by Date, Product, Segment, and Region.



Navigation: Custom buttons and Bookmarks for a seamless multi-page experience.



4\. Advanced Features



Top N Analysis: Identified Top N Products by Sales and Top N Customers by Profit.



Drill through: Enabled deep-dive analysis into specific data points.



Row-Level Security (RLS): Defined roles for Region Managers to view localized data.



Color Palette (Used for Theme)



Light Blue: #A6C3E6



Coral: #F5B499



Warm Yellow: #FFD891



Sage Green: #B1D2A2



Slate Grey: #979EB4



Mobile Layout



The report has been optimized for mobile viewing, prioritizing KPI cards and Top N visuals for on-the-go analysis.

