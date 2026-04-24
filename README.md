# Tata-Data-Visualisation-Empowering-Business-with-Effective-Insights

## Project Description
## Overview
Tata Data Visualisation: Empowering Business with Effective Insights is a comprehensive data analytics project focused on the global performance of an online retail entity. This project simulates a professional consultancy engagement where the end goals are defined by the strategic needs of the CEO and CMO. By utilizing the full suite of Microsoft Power BI, I converted over 500,000 rows of transactional data into a focused narrative to guide the company's international expansion and marketing optimization.

## Technical Stack: Power BI Ecosystem
The project was executed entirely within Power BI, utilizing three distinct layers of the platform:

Power Query (M Language): For complex ETL (Extract, Transform, Load) processes and data structural integrity.

DAX (Data Analysis Expressions): For creating high-performance measures, calculated columns, and time-intelligence calculations.

Visualization : For crafting an intuitive, interactive dashboard that facilitates executive discovery.

## The Deep-Dive Approach
1. Data Engineering with Power Query
Before visualization, a robust data foundation was built through several transformation steps:

Data Cleansing: Implemented conditional filters to exclude non-commercial transactions (quantities < 0 and unit prices <= 0), ensuring the revenue figures were not skewed by returns or internal adjustments.

Data Type Standardisation: Applied strict typing to InvoiceDate, Quantity, and UnitPrice to ensure calculation accuracy in the DAX engine.

Dimensionality: Extracted time-based attributes (Year, Month, Hour, Day of Week) from the InvoiceDate column to allow for granular seasonality and hourly traffic analysis.

Profiling: Used "Column Quality" and "Column Distribution" tools to identify and handle null values in the CustomerID field, ensuring accurate segmentation without losing overall revenue totals.

2. Analytical Logic with DAX
I developed custom DAX measures to move beyond basic counts and sums, providing deeper business context:

Total Revenue: Created a robust measure using SUMX(Sales, [Quantity] * [UnitPrice]) to ensure per-line accuracy.

Time Intelligence: Utilized SAMEPERIODLASTYEAR and TOTALYTD functions to compare growth patterns and identify the Q4 revenue surge.

Customer Loyalty Metrics: Developed a "Customer Count" measure using DISTINCTCOUNT(Sales[CustomerID]) and compared it against total orders to calculate the 98.9% Retention Rate.

AOV (Average Order Value): Leveraged a ratio measure [Total Revenue] / [Total Orders] to identify high-value regions like the Netherlands vs. high-volume regions like the UK.

3. Strategic Visualisation & Insight Generation
The dashboard was designed using "User-Centric Design" principles, categorized for specific leaders:

The CEO View: Focused on global revenue distribution. Used Map Visuals and Ranked Bar Charts to highlight that while the UK is the core market, the European segment (Germany, EIRE, France) presents the highest scalability with lower operational overhead.

The CMO View: Focused on consumer behavior. Developed an Hourly Sales Line Chart to pinpoint the 10 AM – 3 PM "Golden Window" and a Top 10 Product Matrix to suggest cross-selling opportunities for best-sellers like "Jumbo Bags" and "Gliders."

Expansion Modeling: Used Slicers for Region and Time to allow the leadership team to "stress-test" different expansion scenarios by viewing performance in specific months across different international territories.

## Key Project Outcome
By staying within the Power BI ecosystem, I ensured that the project remains a dynamic tool. The underlying Power Query logic and DAX measures mean the dashboard can be updated instantly with new data, providing the CEO and CMO with a living resource for their expansion strategy rather than a static report.
