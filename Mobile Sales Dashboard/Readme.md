**📱 Mobile Sales Dashboard – Power BI Project (DAX-Driven)**

**📝 Project Overview**
This project is a Power BI interactive dashboard built for analyzing mobile phone sales data. The key focus of this project is on using DAX (Data Analysis Expressions) to create advanced calculations for insights into product performance, revenue trends, and business KPIs.

**🎯 Objectives**

Visualize mobile sales trends over time.

Analyze product-wise and brand-wise performance.

Use DAX to create calculated metrics and measures.

Compare regional and store-level sales performance.

Identify profitable products and discount impact.

**📁 Dataset Description**

The dataset used contains mobile phone sales records with the following columns:

Order ID

Order Date

Brand

Model

Category (e.g., Smartphone, Feature Phone)

Quantity Sold

Unit Price

Discount

Revenue

Profit

Store Name

Region

**🔄 Data Preparation**

Data was preprocessed in Power Query with the following steps:

Removed duplicate and null values

Converted data types (dates, currency, numbers)

Added calculated columns like Year, Month, and Discounted Price

Created relationships (Star Schema) between:

Date table

Sales table

Product table

Region/Store table

**🧠 DAX Measures Used**

Here are examples of key DAX measures created:

dax
Copy
Edit
Total Revenue = SUM(Sales[Revenue])

Total Profit = SUM(Sales[Profit])

Total Quantity = SUM(Sales[Quantity Sold])

Average Selling Price = DIVIDE([Total Revenue], [Total Quantity])

Profit Margin % = DIVIDE([Total Profit], [Total Revenue]) * 100

Discount Impact = SUMX(Sales, Sales[Discount] * Sales[Quantity Sold])

YoY Growth = 
VAR CurrentYear = [Total Revenue]
VAR PreviousYear = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('Date'[Date]))
RETURN DIVIDE(CurrentYear - PreviousYear, PreviousYear) * 100

**📊 Key Visuals in the Dashboard**

📆 Time Series Line Chart – Revenue trend over months/years

📌 Bar Chart – Top 10 best-selling mobile models

🏬 Store/Region Map – Revenue by region

🛒 Stacked Column Chart – Brand-wise comparison

💵 KPI Cards – Total Sales, Profit, Units Sold, Profit Margin

🔍 Slicers – Date, Brand, Category, Store, Region

**📌 Features**

Clean, user-friendly dashboard design

Slicers and filters for dynamic user exploration

Drill-through functionality on product and store

Hover tooltips with DAX metrics for context

Month-over-Month and Year-over-Year comparison

**📈 Key Insights**

Smartphones account for over 80% of total revenue.

Brand X and Brand Y dominate the sales market.

Discounted sales have a clear impact on profit margins.

Region South shows the highest YoY growth in mobile sales.

**⚙️ Tools & Technologies Used**

Power BI Desktop

Power Query

DAX (Data Analysis Expressions)

Microsoft Excel / CSV (for data source)

**🚀 Future Improvements**

Add forecasting using Power BI’s AI capabilities

Integrate live database for real-time analytics

Develop customer segmentation based on purchase history

Enable mobile view optimization

**📬 Contact**
Created by: Yashraj Ghanvat
Email: ghanvatyashraj@gmail.com
LinkedIn: www.linkedin.com/in/yashraj-ghanvat-981985269

