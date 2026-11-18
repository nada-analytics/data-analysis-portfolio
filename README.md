 Superstore Sales Data Cleaning & Analysis

 1. Objective:
To clean, prepare, and analyze the Superstore Sales dataset in order to answer key business questions regarding sales performance, profit margins, and regional trends.

 2. Dataset:
- Source: Superstore Sales dataset (Excel format).
- Structure: Contains multiple rows and columns including Order Date, Product Name, Category, Sales, Profit, Quantity, and Region.

 3. Data Cleaning & Analysis Steps:
- Removed duplicate records to ensure data integrity.
- Standardized text fields using PROPER and TRIM functions.
- Fixed date formatting and removed timestamp errors.
- Created a Profit Margin column using formulas and formatted it as percentages.

      
 4. Insights:
-Geographic Sales Performance
  Insight: Sales and orders are concentrated heavily in specific regions while other areas show very low activity.
 Recommendation: Focus marketing campaigns and special offers on low-performing regions to increase market share

-Category Profitability
 Insight: Some product categories generate high sales volume but low profit margins while others bring good profits with fewer sales
 Recommendation: Review discount strategies on high-sales items and promote products with higher profit margins

-Monthly Sales Trends
 Insight: Sales peak significantly during certain months of the year followed by noticeable drops during slow periods
 Recommendation: Prepare inventory and shipping capacity ahead of peak months and offer discounts during slow months to maintain steady revenue

5. Challenges & Solutions:
   Challenge: Handling messy dates and inconsistent text formats in the raw dataset.
   Solution: Cleaned and standardized text fields using PROPER and TRIM functions, and fixed date formatting errors.

<img width="1366" height="768" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/2c7413e3-88b1-4e0c-906b-f3a8cdc13f0e" />
<img width="1366" height="768" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/3da0ff5b-6dc1-4bc5-a2fb-d72c9d29e512" />
<img width="1366" height="768" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/0945724f-3a1c-495b-85e7-f8ecdc2ee156" />
6. Power BI Data Preparation (Day 4):
Imported the cleaned Excel dataset into Power BI Desktop and opened Power Query Editor via Transform Data.
Verified all column data types (Text, Date, Number) and inspected column headers.
Removed a corrupted column whose header contained unreadable symbols/characters.
Dropped additional unneeded columns to keep only relevant fields for dashboard analysis.
 Applied all transformations using Close & Apply.
  <img width="1366" height="768" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/ca72eaba-a843-4cd1-830d-46e64e1af715" />
