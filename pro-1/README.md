#### Project: Data Leverager





1\. Data Extraction :



\-> I loaded data from three different sources:



* Web Data: Loaded an HTML table from the web for country-wise GDP.
* Folder Source: Combined 3 monthly Sales files (Jan, Feb, and Mar) from a single folder.
* Excel/CSV File: Loaded an employee dataset containing details like Employee ID and Department.





2\. Basic Transformations : 



\-> I cleaned the raw data to make it ready for analysis:



* Removing Waste: Deleted all blank rows, blank columns, and duplicate records to keep only useful data.
* Setting Headers: Used the first row as "Headers" so each column has a proper name.
* Naming Columns: Renamed columns to simple, meaningful names that are easy to understand.
* Fixing Data Types: Changed data formats (like Date and Currency) using Locale settings to avoid errors.
* Fixing Data Types: Changed data formats (like Date and Currency) using Locale settings to avoid errors.





3\. Text Tools :



\-> I checked if the data is correct and healthy:



* Fixing Case: I used UPPER() and LOWER() to make customer names and categories look consistent.
* Cleaning Text: I used TRIM() and CLEAN() to remove extra spaces and hidden characters from the text.
* Updating Info: I used REPLACE() to fix wrong values in the dataset.
* Splitting Address: I used SPLIT COLUMN BY DELIMITER to separate the address into City and Region.





4\. Numeric Tools:



\-> I worked with numbers and math to get more insights from the data:



* Rounding Numbers: I rounded the revenue columns to 2 decimal places to make the numbers look clean and professional.
* Calculating Profit: I created a new column to calculate Profit by subtracting Cost from Revenue ($Profit = Revenue - Cost$).





5\. Date \& Time Tools:



\-> I used date functions to create better time-based information:



* Extracting Details: I pulled out the Day, Month, Year, and Quarter from the "Order Date" column to analyze sales by time periods.
* Fiscal Month: I created a custom Fiscal Month column using the "Add Column" feature to match the business calendar.
* Age Calculation: I added a new column to calculate the Age of employees using their "Birthdate".





6\. Conditional Columns \& Indexing: 



\-> I added logic to categorize the data and numbered the rows for better tracking:



* Sales Category: I created a new column to automatically label sales based on revenue:
* High: Sales >= 10,000
* Medium: Sales between 5,000 and 9,999
* Low: Sales < 5,000
* Index Columns: I added 0-based and 1-based index columns to give a unique number to every row in the dataset.





7\. Pivoting \& Unpivoting :



\-> I changed the structure of the table to make it better for analysis:



* Unpivoting Columns: I turned the separate monthly columns (Jan, Feb, Mar) into one single "Month" column.
* Normalizing Data: This process helps in organizing the data into a standard format, which is much easier to use for creating charts and filters.





8\. Merging \& Appending :



\-> I combined different data tables to create a complete dataset:



* Combining Sales: Since I kept all monthly sales files (Jan, Feb, Mar) in one folder, I used Append Queries to join them into one master list.
* Connecting Data: I merged the Sales data with the Employee list using Employee ID. This allows me to see which employee made which sale.





9\. Grouping \& Aggregation :



\-> I summarized the data to see the performance of each region:



* Group by Region: I grouped the data by "Region" and calculated these three values:
* Total Sales: Sum of all revenue for each region.
* Average Order Value: The average amount spent per order.
* Transaction Count: Total number of orders in each region.



* East Region:                                   



&#x20;  Total Sales: 1,584,395

&#x20;  Average Order Value: 5,559.28

&#x20;  Transaction Count: 285



* Central Region:



&#x20;  Total Sales: 1,677,406

&#x20;  Average Order Value: 5,499.69

&#x20;  Transaction Count: 305



* West Region:



&#x20;  Total Sales: 1,554,883

&#x20;  Average Order Value: 5,513.76

&#x20;  Transaction Count: 282



* South Region:



&#x20;  Total Sales: 1,712,493

&#x20;  Average Order Value: 5,542.04

&#x20;  Transaction Count: 309



* North Region:



&#x20;  Total Sales: 1,664,181

&#x20;  Average Order Value: 5,641.29

&#x20;  Transaction Count: 295



=> Note: I deleted the 'Grouped Rows' step to get back the full data for my report.





10\. Data Profiling \& Quality : 



\-> I checked if the data is correct and healthy:



* Finding Errors: I used Column Quality to find and fix any missing values or errors.
* Understanding Data: I used Column Profile and Distribution to see unique values and ensure data accuracy.





11\. Source Settings \& Parameters : 



\-> I made the project "smart" so it can work on any computer without breaking:



* Dynamic Folder Path: I created a Parameter for the folder path. This helps to change the data location easily in one click.
* Data Source Settings: I managed the file permissions and paths under Data Source Settings to ensure a smooth connection to the data.





12\. Refresh Simulation :



\-> In this final step, I tested the automation of the project:



* Auto-Load Test: I added a new monthly file (e.g., Sales\_ Apr) to the folder to see if Power BI picks it up automatically.
* Verify Refresh: I clicked the Refresh button and confirmed that all my cleaning steps (Transformations) were applied to the new data without any extra work.





























































