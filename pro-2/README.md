

### Data Modeler :-





* Data Acquisition \& Loading

&#x20;  - Instruction: Load the provided datasets into Power BI Desktop.

&#x20;  - What I did: I imported all the CSV/Excel files (Sales, Returns, Products, Customers, Regions, and Date) into Power BI using the 'Get Data' feature.





1\. Advanced Model Settings (How I did it):



&#x20;  - Instruction: Set appropriate relationship cardinalities.

&#x20;  - What I did: I connected the Dimension tables to Fact tables using a 1:Many relationship.



&#x20;  - Instruction: Set cross-filter directions (preferably single).

&#x20;  - What I did: I set all relationship arrows to 'Single' direction to keep the data flow clear.



&#x20;  - Instruction: Enable and disable bidirectional filters only where justified.

&#x20;  - What I did: I avoided bidirectional filters to prevent confusion in the data model.



&#x20;  - Instruction: Simulate inactive relationship scenarios using the Returns\_Fact table.

&#x20;  - What I did: I created a dotted (inactive) line between Returns\_Fact and Date\_Dim using the ReturnDateKey.



&#x20;  - Instruction: Identify and resolve any filter ambiguity issues.

&#x20;  - What I did: I kept the secondary date connection 'Inactive' so Power BI doesn't get confused between Sales and Returns dates.





2\. Data Model Enhancements (Extra value I added):



&#x20;  - Instruction: Set appropriate data formats (e.g., currency, whole numbers, dates).

&#x20;  - What I did: I formatted the Revenue and Discount columns to Currency (₹) and set Quantity as a Whole Number.



&#x20;  - Instruction: Define Data Categories (e.g., City, Country).

&#x20;  - What I did: I marked the City and Country columns with Geographic categories so they work perfectly on Maps.



&#x20;  - Instruction: Build Date Hierarchy (Year > Quarter > Month > Date).

&#x20;  - What I did: I created a Date Hierarchy in the Date\_Dim table for easy time-based analysis.



&#x20;  - Instruction: Build Region Hierarchy (Country > State > City).

&#x20;  - What I did: I built a Region Hierarchy to allow users to drill down from Country level to City level.



&#x20;  - Instruction: Build Product Hierarchy (Category > Subcategory > ProductName).

&#x20;  - What I did: I organized products into a Product Hierarchy to see sales from broad categories down to specific items.





3\. Verification Step (Final Results):



&#x20;  - Instruction: Use a Matrix Table to verify Sales by Product Category and Region.

&#x20;  - What I did: I created a Matrix visual that successfully showed different Sales totals for each Category and Country.



&#x20;  - Instruction: Verify Return reasons by Fiscal Year.

&#x20;  - What I did: I used a Matrix to confirm that the Inactive relationship is working and showing correct return counts per year.



&#x20;  - Instruction: Verify Revenue by Customer Segment.

&#x20;  - What I did: I checked the Revenue for Gold, Platinum, and Silver segments, and the Total matched with the overall sales.





* Star Schema vs. Snowflake Schema: 



&#x20;  - Star Schema: In this model, all Dimension tables connect directly to the central Fact table. It is very fast and makes reports load quickly in Power BI.



&#x20;  - Snowflake Schema: In this model, Dimension tables are split into more sub-tables. It is more complex and can sometimes make the report slower.



&#x20;  - Conclusion: I used the Star Schema for this project because it is simple to manage and gives the best performance in Power BI.





* Relationship Rationale: To ensure data accuracy between different tables.



* Filter Flow: To control how one table filters another without creating confusion.





* Resolved Filter Ambiguity by using inactive relationships.



* Fixed Map errors by assigning proper Data Categories.



* Improved Readability by applying correct currency formatting.





































































