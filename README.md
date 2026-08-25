# Food-Delivery-Analysis-Power-BI
🍔 Food Delivery Analysis & Dashboard

An end-to-end Business Intelligence (BI) study utilizing synthetic dataset generation, Power Query ETL pipelines, advanced DAX modeling, and interactive Power BI dashboards.

# 📌Executive-Summary

This project presents a comprehensive analytics solution for a multi-city food delivery service. The objective was to transform raw transactional data into actionable operational and financial insights by evaluating:

📦 Order volumes
💰 Revenue performance
⭐ Customer satisfaction
🚴 Delivery efficiency
🌍 Regional market distribution
#📊 Key Metrics
Metric                          Value
📦 Total Orders Processed	  51
💰 Total Revenue      	  $27K
⭐ Average Customer Rating	  3.63 / 5.0
🌍 Geographic Coverage	  10 Major Indian Cities
#👥 Team & Responsibilities
Contributor	Primary Role	Core Execution
Saad Shaikh	🧹 Data Cleaning & Preparation	Dataset ingestion, structure alignment, duplicate elimination, and missing-value handling using Power Query.
Rechal Parshee	📈 DAX & Analysis	Data modeling, time-intelligence DAX formulation, and statistical relationship definitions.
Soham Deshmukh	🎨 Dashboard & UI	UX visual architecture, KPI configuration, theme design, and final Power BI dashboard publishing.
#🛠️ Technical Architecture & Tools
# 1.🤖 Dataset Generation — ChatGPT

Prompt-engineered raw food-delivery ordering logs simulating real-world transactional data, including:

Order IDs
Order dates
Cities
Delivery times
Customer ratings
Restaurant categories
Order values
#2. 🔄 Data Preparation — Power Query

An automated ETL pipeline was developed to:

Clean and transform raw data
Standardize data types
Rename and align columns
Handle missing attributes
Remove duplicate records
Standardize text casing
#3. 📐 Analytical Modeling — Power BI & DAX

Custom DAX measures were created to support executive-level decision-making, KPI tracking, and period-over-period analysis.

#🔁 Workflow & Data Pipeline
Synthetic Dataset Generation
          ↓
     Data Ingestion
          ↓
   Power Query ETL
          ↓
 Data Cleaning & Transformation
          ↓
   Schema Optimization
          ↓
    DAX Data Modeling
          ↓
 Interactive Power BI Dashboard

#Workflow Steps
Dataset Generation: Simulated transactional logs across multiple food categories and Indian cities.
Power Query Pipeline: Imported data into Power BI Desktop, handled null values, transformed data types, and removed duplicate records.
Schema Optimization: Structured fact and dimension relationships for cities, categories, and restaurants.
Interactive Dashboard Development: Created both Light Mode and Dark Mode interfaces with slicers, cross-filtering, and drill-down functionality.
#🗂️ Power BI Data Model Schema
Field Name	Data Type	Role / Structure	Business Context
Order ID	Text / Key	Primary Dimension	Unique transaction code for tracking orders
Order Value / Revenue	Decimal Currency	Fact / Aggregation	Base measure for Total Revenue
Delivery Time	Integer (Minutes)	Fact Metric	Used to analyze logistics speed across cities
Rating	Decimal (1.0–5.0)	Fact Metric	Used to calculate customer satisfaction
Revenue Growth %	Percentage Measure	DAX Time Intelligence	Period-over-period revenue change
#🧮 Key Performance Measures — DAX
#Total Orders
Total Orders =
COUNT(Orders[Order ID])

#Total Revenue
Total Revenue =
SUM(Orders[Order Value])

#Average Delivery Time
Average Delivery Time =
AVERAGE(Orders[Delivery Time])

#Average Rating
Average Rating =
AVERAGE(Orders[Rating])

#Revenue Growth %

A time-intelligence measure utilizing VAR, OFFSET, and DIVIDE logic to calculate period-over-period revenue variance.

#💡 Key Business Insights
🌍 Geographic Distribution
Kolkata leads total order share with 17.65% (9 orders).
Chennai follows with 15.69% (8 orders).
Bengaluru accounts for 13.73% (7 orders).
#🚴 Fulfillment Speeds

Cumulative delivery time is highest in:

Kolkata: 423 minutes
Chennai: 399 minutes

These figures highlight potential operational bottlenecks within the highest-volume delivery hubs.

#🍕 Category Performance

The dashboard enables interactive analysis across major food categories:

🍜 Street Food
🍔 Fast Food
🍝 Continental
🥘 North Indian
🧁 Desserts & Bakery
🍛 Biryani
🍲 South Indian
🥤 Beverages
🍕
#🎯 Project Outcome

The completed Power BI solution converts raw food-delivery transactions into an interactive business intelligence dashboard, enabling users to monitor revenue, orders, customer satisfaction, delivery efficiency, geographic performance, and food-category trends.

The project demonstrates practical skills in:

Data Cleaning → ETL → Data Modeling → DAX → Visualization → Business Insights
