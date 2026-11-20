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

7. Power BI Measures & Visuals 

Measures Table:
| Measure Name | DAX Formula | Meaning (In My Own Words) |
| :--- | :--- | :--- |
| **Total Sales** | `Total Sales = SUM('Cleaning Log'[Sales])` | Calculates total sales across the dataset and updates dynamically based on selected filters. |
| **Total Profit** | `Total Profit = SUM('Cleaning Log'[Profit])` | Calculates total profit to show overall profitability compared to sales. |
| **Profit Margin** | `Profit Margin = DIVIDE([Total Profit], [Total Sales])` | Shows profit percentage of total sales while safely avoiding division-by-zero errors. |
| **Orders Count** | `Orders Count = DISTINCTCOUNT('Cleaning Log'[Order.ID])` | Counts unique orders so multiple items in the same order are not double-counted. |

Visuals Table:
| Visual / Element | Fields & Measure Used | Meaning (In My Own Words) |
| :--- | :--- | :--- |
| **4 KPI Cards** | `Total Sales`, `Total Profit`, `Profit Margin`, `Orders Count` | Displays key summary numbers at a glance at the top/side of the report. |
| **Column Chart (Sales by Category)** | `Category` (X-axis) & `Total Sales` (Y-axis) | Compares total sales across product categories to show which category generates the most revenue. |
| **Line Chart (Sales by Month)** | `Order.Date` - Month (X-axis) & `Total Sales` (Y-axis) | Tracks how sales rise and fall across months over time. |
| **Bar Chart (Top 10 Products)** | `Product.Name` (Y-axis), `Total Sales` (X-axis), Top 10 filter | Highlights the top 10 highest-selling products for quick identification. |
| **Donut Chart / Map (Sales by Region)** | `Region` & `Total Sales` | Shows how sales are distributed across different regions. |
<img width="1366" height="768" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/9eebebdb-1b6c-4a37-a053-1c3c11fc17d0" />


8. Insights & Recommendations

- Geographic Performance:
  Insight: Sales and orders are higher in certain regions than others showing uneven regional demand.
  Recommendation: Focus marketing and promotions on lower performing regions while keeping stock ready in high demand areas.

 •Category Profitability:
  Insight: Some categories bring high sales while others have lower profit margins or smaller order counts.
  Recommendation: Review discounts on low margin items and promote products that give healthier profit.

•Monthly Sales Trend:
  Insight: Sales go up and down across months with noticeable peaks in specific months of the year.
  Recommendation: Plan inventory and delivery capacity ahead of peak months and run offers during quieter months.

•Top 10 Products:
  Insight: A small group of top products makes up a clear share of overall sales.
  Recommendation: Keep top selling products well-stocked and highlight them to customers.

9. Excel vs. Power BI Comparison:

Both Excel and Power BI helped me analyze this dataset, but each one is better for different tasks:
- Difference: Excel is great for quick data cleaning cell formulas  and Pivot Tables while Power BI connects data preparation in Power Query with DAX, measures, slicers, cross-filtering visuals, and multi-page reports.
- Which felt easier: Excel felt easier at the beginning for fast manual checks and simple tables while Power BI felt easier and faster for building an interactive dashboard and filtering results visually across charts.

 <img width="1366" height="768" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/1fe304d3-5029-46e8-8eb4-7a5c57022b1e" />
<img width="1366" height="768" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/d4bd879b-1f58-47ae-8537-da34f9eccf97" />
