#Vishal Mega Mart Sales Dashboard – Power BI Project
📊 Project Overview
This Power BI project aims to analyze and visualize sales data from Vishal Mega Mart, a leading retail chain in India. The goal is to uncover insights on revenue trends, store performance, product sales, and customer behavior to support data-driven decision-making.

🎯 Objectives
Visualize monthly and yearly sales performance.

Identify top-performing stores and products.

Track key business metrics such as profit, quantity sold, and discounts.

Analyze customer behavior and regional trends.

Provide interactive filters for user-driven insights.

📁 Dataset Used
Source: Internal sales records or public datasets (if using mock data).
Data Fields may include:

Order Date

Product Name

Category & Sub-Category

Store Location

Quantity Sold

Sales

Profit

Discount

Customer ID

🔧 Data Preprocessing
Performed using Power Query and included:

Removing null and duplicate records

Changing data types

Creating calculated columns (e.g., profit margin, month-year)

Building relationships between tables (star schema)

📊 Key Visualizations
KPI Cards for Total Sales, Profit, Quantity Sold

Line Charts for Monthly Sales Trends

Bar Charts for Top 10 Stores & Products

Map for Regional Sales Distribution

Pie/Donut Charts for Category-wise Sales

Slicers/Filters for Year, Store, Category, etc.

📈 Dashboard Features
Fully interactive with slicers for dynamic filtering

Clean and business-friendly UI

Drill-down capabilities to explore data from high-level to detailed views

📐 DAX Measures Created
Some custom DAX measures:

Total Sales = SUM(Sales[Amount])
Total Profit = SUM(Sales[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales])
Sales Trend = CALCULATE([Total Sales], DATESYTD('Date'[Date]))
🧪 Evaluation Metrics
Monthly Sales Growth %

Profit Margin %

YoY and MoM comparisons

Store-wise sales contribution

💡 Key Insights
North and West zones generate the highest revenue.

Electronics and Apparel are the most profitable categories.

Discounts above 20% reduce overall profit margins.

Few stores underperform despite high footfall – need optimization.

📌 Tools Used
Power BI Desktop

Power Query Editor

DAX for custom measures

Excel/CSV (for data input)

🚀 Future Enhancements
Incorporate customer segmentation

Forecasting sales using built-in Power BI forecasting tools

Real-time dashboard with live database connection

📬 Contact
For queries, feel free to contact:
Name: Yashraj Ghanvat
Email: ghanvatyashraj@gmail.com
LinkedIn: www.linkedin.com/in/yashraj-ghanvat-981985269
