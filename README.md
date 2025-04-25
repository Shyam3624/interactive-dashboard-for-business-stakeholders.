**✅ Key Features Implemented**

**1. 📌 KPIs Selection**

Total Sales: Derived using SUM(Sales)

Estimated Profit: Calculated using the DAX measure Profit = [Sales] - [Cost]

Year-over-Year (YoY) Sales Growth:

DAX
Copy
Edit
YoY Sales Growth (%) = 
DIVIDE([Total Sales] - CALCULATE([Total Sales], DATEADD('Orders'[Order Date], -1, YEAR)), 
CALCULATE([Total Sales], DATEADD('Orders'[Order Date], -1, YEAR))) * 100


**2. 🎛️ Slicers / Filters for Interactivity**

Region – To view sales/profit trends across different geographic zones.

Segment – To analyze sales by Customer Segment (e.g., Consumer, Corporate).

Ship Mode – To filter based on different shipping methods.

Order Date – Enabled filtering by Year/Quarter/Month using date hierarchy.

**3. 📈 Time-Series Analysis**

Created line and area charts for Sales across time.

Utilized DAX date intelligence to enable dynamic year/month-level trend comparisons.

**4. 🧮 Custom Calculated Columns & Measures**

Profit was calculated as:

DAX
Copy
Edit
Profit = Sales - Cost
Average Sales per Order:

DAX
Copy
Edit
Avg Sales per Order = AVERAGEX(VALUES('Orders'[Order ID]), [Sales])

**5. 📇 Cards for Totals & Summary**

Used Power BI card visuals to display:

Total Sales

Total Profit

Average Sales per Order

YoY Growth %

Each card uses dynamic measures and updates with slicer interaction.

**6. 🎨 Consistent Color Theme**

Applied a corporate-style color theme using:

Shades of blue for sales

Green for profit metrics

Gray for background visuals

Ensured uniform fonts and visual alignment across all pages.

**7. 🧭 Navigation Menu**

Created using Power BI Buttons and set Action → Page Navigation to switch between:

Overview

Detailed Analysis

Time Trend Page

Each button enables a seamless interactive experience for users.

**💻 Tools Used**

Microsoft Power BI Desktop

DAX for calculated measures

GitHub for version control and presentation sharing
