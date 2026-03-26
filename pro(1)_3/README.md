### **Project Name: DAX Depo - End-to-End Sales Analytics**



###### **Project Description**



This project demonstrates a complete Power BI development lifecycle. It involves transforming raw Sales and Returns data into a professional analytical report using advanced DAX (Data Analysis Expressions).



###### **Key Project Milestones (Tasks 1-12)**



**1. Data Cleaning \& Transformation (Tasks 1-4)**

* Cleaned **Sales\_ Fact, Customer\_ Dim**, and **Product\_ Dim** tables.
* Handled null values and removed duplicates to ensure data accuracy.
* Created a dedicated **Date\_ Dim** (Calendar Table) for time-based analysis.





**2. Data Modeling \& Relationships (Task 5)**



* Established a **Star Schema** model.
* Created **One-to-Many relationships** between Dimension tables and the Fact table.





**3. Dedicated Measure Management (Task 6)**



* Created a **Dedicated Measure Table** (Key Measures) to keep all DAX calculations organized in one place.





**4. Basic \& Advanced DAX Measures (Tasks 7-8)**



* Created core metrics: Total Sales, Total Cost, and Total Profit.
* Used **Iterator Functions** like SUMX and AVERAGEX for row-level profit calculations.
* Implemented counting functions like DISTINCTCOUNT for unique customer tracking.





**5. Filter Context \& Logic (Tasks 9 \& 11)**



* Used **CALCULATE, ALL,** and **KEEPFILTERS** to compare regional sales against grand totals.
* Applied **Logical Functions** (IF, AND, OR, SWITCH) to create a **Performance Tag** column (categorizing sales as Excellent, Good, or Low).





**6. Time Intelligence Analytics (Task 10)**



**=>** Developed time-based insights using:



* TOTALYTD for Year-to-Date sales tracking.
* SAMEPERIODLASTYEAR for year-over-year (YoY) growth comparison.
* **Running Totals** to see cumulative sales progress.





**7. Final Output \& Optimization (Task 12)**



* Organized measures into **Display Folders.**
* Built a dynamic **Matrix Visual** that allows drilling down from Region to Performance Tags.
* Verified report speed using the **Performance Analyzer.**





**Tools Used**



* Power BI Desktop: Report building and visualization.
* Power Query: Data cleaning and ETL.
* DAX: Advanced analytical calculations.





**How to View the Report**



* Open the .pbix file in Power BI Desktop.
* Navigate to the Matrix Visual to see Regional and Performance breakdowns.
* Check the Key Measures table for all the logic used in this project.

