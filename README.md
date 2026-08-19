🏠 Real-Estate-Property-Analytics-Dashboard

Built an interactive Real Estate Property Analytics Dashboard in Microsoft Power BI using Power Query, DAX, Data Modeling, KPI Cards, Charts, Maps, and Slicers. Analyzed property prices, locations, property types, bedrooms, bathrooms, property sizes, furnishing, amenities, and construction information to generate actionable real estate insights.

An interactive Real Estate Property Analytics Dashboard built in Microsoft Power BI to analyze property prices, city and locality performance, property characteristics, amenities, and market trends. This project demonstrates an end-to-end data analysis workflow, from data cleaning and EDA to dashboard creation and business insights.

🔍 Exploratory Data Analysis (EDA)
Exploratory Data Analysis was performed on the Real Estate Property dataset to understand property prices, locations, property characteristics, amenities, and relationships between different variables before creating the Power BI dashboard.

📊 1. Dataset Overview

The dataset contains real estate property information including:

City Locality Bedrooms Bathrooms Living area Lot area Floors Property type Furnishing Parking Lift Balcony Garden Nearby schools Nearby hospitals Construction year Renovation year Property price 🧹 2. Data Quality Check

The following checks were performed:

Checked total rows and columns. Checked column names. Checked data types. Checked missing values. Checked duplicate records. Checked invalid values. Checked numerical ranges. Checked categorical values. Checked property price values. 💰 3. Property Price Analysis

Analyzed:

Minimum property price Maximum property price Average property price Property price distribution High-value properties Low-value properties Purpose

To understand the overall property market and identify price variations.

🌆 4. City-Wise Analysis

Analyzed property distribution and pricing across different cities.

Analysis Number of properties by city Average price by city Minimum price by city Maximum price by city City-wise property distribution Business Question

Which cities have the highest and lowest average property prices?

📍 5. Locality-Wise Analysis

Analyzed property prices across different localities.

Analysis Properties by locality Average locality price Top expensive localities Affordable localities Business Question

Which localities are the most expensive?

🏠 6. Property Type Analysis

Analyzed different property types.

Examples:

Apartment Villa House Other available property categories Analysis Property count by type Average price by type Price distribution by type 🛏️ 7. Bedroom Analysis

Analyzed the number of bedrooms in properties.

Analysis Property count by bedrooms Average price by bedrooms Price distribution by bedrooms Business Question

Does the number of bedrooms affect property prices?

🚿 8. Bathroom Analysis

Analyzed the number of bathrooms.

Analysis Property count by bathrooms Average price by bathrooms Comparison between bathrooms and price 📏 9. Living Area Analysis

Analyzed sqft_living.

Analysis Average living area Minimum living area Maximum living area Living area distribution 📈 10. Living Area vs Property Price

A relationship analysis was performed between:

sqft_living ↓ property price Visualization

Scatter Plot

Purpose:

Understand whether larger properties tend to have higher prices.

🌳 11. Lot Area Analysis

Analyzed sqft_lot.

Analysis Minimum lot area Maximum lot area Average lot area Lot area vs property price 🏢 12. Floors Analysis

Analyzed the number of floors.

Analysis Property count by floors Average price by floors Price distribution by floors 🛋️ 13. Furnishing Analysis

Analyzed furnishing categories.

Analysis Furnished properties Semi-furnished properties Unfurnished properties Average price by furnishing Business Question

Does furnishing status influence property price?

🚗 14. Parking Analysis

Analyzed parking availability.

Analysis Properties with parking Properties without parking Average price based on parking 🛗 15. Lift Analysis

Analyzed lift availability.

Analysis Properties with lift Properties without lift Price comparison 🌿 16. Balcony Analysis

Analyzed balcony availability/count.

Analysis Properties with balconies Properties without balconies Average price comparison 🌳 17. Garden Analysis

Analyzed garden availability.

Analysis Properties with gardens Properties without gardens Average price comparison 🏫 18. Nearby Schools Analysis

Analyzed the number of nearby schools.

Purpose

To understand whether properties have better access to educational facilities.

🏥 19. Nearby Hospitals Analysis

Analyzed nearby hospitals.

Purpose

To understand the availability of healthcare facilities around properties.

🏗️ 20. Year Built Analysis

Analyzed property construction years.

Analysis Old properties New properties Property count by construction year Average price by construction year 🔨 21. Year Renovated Analysis

Analyzed renovation information.

Analysis Renovated properties Non-renovated properties Average price comparison 🧩 22. Correlation Analysis

Relationships between numerical variables can be analyzed, including:

sqft_living ↔ price sqft_lot ↔ price bedrooms ↔ price bathrooms ↔ price floors ↔ price year_built ↔ price

Purpose:

Identify relationships between property characteristics and price.

📌 23. EDA Summary

The EDA helped identify:

Property price patterns. City-wise pricing differences. Locality-wise pricing differences. Property type distribution. Bedroom and bathroom patterns. Relationship between property size and price. Furnishing differences. Amenity availability. Construction and renovation patterns.

📸 EDA Preview image image image image image image image image image image image image image image image image image image

📌 Project Overview
This project transforms raw real estate property data into an interactive dashboard that helps users understand property pricing and market characteristics.

The dashboard provides insights into:

Property prices
Average property price
City-wise property distribution
Locality-wise pricing
Property types
Bedroom and bathroom distribution
Living area and lot size
Furnishing status
Parking availability
Lift availability
Balcony and garden availability
Nearby schools and hospitals
Construction year
Renovation year
📊 Power BI Dashboard
🎯 Objectives
Clean and transform raw real estate data.
Perform exploratory data analysis (EDA).
Create meaningful KPIs.
Analyze property prices across cities and localities.
Identify high-value and affordable areas.
Understand the relationship between property size and price.
Build dynamic charts and interactive visualizations.
Create a geographic property price analysis.
Design an interactive Power BI dashboard.
Generate actionable business insights.
🛠️ Tools Used
Microsoft Power BI
Power Query
DAX
Microsoft Excel / CSV
Data Modeling
KPI Cards
Slicers
Maps
Charts
Data Visualization
📊 Dashboard KPIs
🏠 Total Properties
💰 Total Property Value
💵 Average Property Price
💎 Maximum Property Price
📉 Minimum Property Price
🌆 Total Cities
📍 Total Localities
📏 Average Living Area
🛏️ Average Bedrooms
🚿 Average Bathrooms
📈 Dashboard Visualizations
KPI Cards
Property Price by City
Top 10 Localities by Average Price
Property Type Distribution
Price by Bedrooms
Price by Bathrooms
Property Price Map
Living Area vs Price
Lot Area vs Price
Furnishing Analysis
Parking Analysis
Lift Availability
Balcony Availability
Garden Availability
Year Built Analysis
Year Renovated Analysis
🧹 Data Cleaning & Transformation
The raw dataset was cleaned and transformed using Power Query.

Data Cleaning Steps
Imported the raw CSV/Excel dataset.
Checked the number of rows and columns.
Checked missing values.
Removed duplicate records.
Corrected data types.
Standardized city names.
Standardized locality names.
Checked invalid property prices.
Checked bedroom and bathroom values.
Checked property-size values.
Standardized categorical columns.
Checked year-built values.
Checked year-renovated values.
Removed unnecessary data where required.
Loaded the cleaned data into Power BI.
🗺️ Property Price Map
A map visualization was created to analyze property prices geographically.

Map Configuration
Location → City
Size → Average Property Price
Legend → Property Type
Tooltips → Price
             Bedrooms
             Bathrooms
             Sqft Living
             Property Type
Note
The dataset contains city and locality information but does not contain latitude and longitude. Therefore, the map provides city-level geographic analysis rather than exact property-level locations.

🧮 Important DAX Measures
Total Properties
Total Properties =
COUNTROWS(RealEstate)
Total Property Value
Total Property Value =
SUM(RealEstate[price])
Average Property Price
Average Property Price =
AVERAGE(RealEstate[price])
Maximum Property Price
Maximum Property Price =
MAX(RealEstate[price])
Minimum Property Price
Minimum Property Price =
MIN(RealEstate[price])
Total Cities
Total Cities =
DISTINCTCOUNT(RealEstate[city])
Total Localities
Total Localities =
DISTINCTCOUNT(RealEstate[locality])
Average Living Area
Average Living Area =
AVERAGE(RealEstate[sqft_living])
Average Bedrooms
Average Bedrooms =
AVERAGE(RealEstate[bedrooms])
Average Bathrooms
Average Bathrooms =
AVERAGE(RealEstate[bathrooms])
📂 Dataset
Dataset Name: Real Estate Property Dataset

Dataset columns:

city
locality
bedrooms
bathrooms
sqft_living
sqft_lot
floors
year_built
year_renovated
property_type
parking
facing
lift
furnishing
nearby_schools
nearby_hospitals
society
balcony
garden
price
Place the dataset in the project folder:

indian_house_prices.csv
## 🚀 Project Workflow

### Step 1

Import the real estate dataset.

### Step 2

Clean and transform data using Power Query.

### Step 3

Check missing values and duplicate records.

### Step 4

Correct data types and standardize categorical values.

### Step 5

Perform exploratory data analysis.

### Step 6

Create the Power BI data model.

### Step 7

Create DAX measures.

### Step 8

Create KPI cards.

### Step 9

Build charts and map visualizations.

### Step 10

Add interactive slicers and filters.

### Step 11

Design the dashboard layout.

### Step 12

Validate KPI values and visualizations.

### Step 13

Generate business insights.

---

## 🎛️ Interactive Filters

The dashboard includes interactive slicers for:

* City
* Locality
* Property Type
* Bedrooms
* Bathrooms
* Furnishing
* Facing
* Floors
* Year Built
* Year Renovated
* Parking
* Lift
* Balcony
* Garden
---
📸 Dashboard Preview
Screenshot 2026-08-12 103625 Screenshot 2026-08-09 220320 Example:
Images/Real_Estate_Property_Dashboard.png
📁 Repository Structure
Real-Estate-Property-Analytics-Dashboard/
│
├── Real_Estate_Property_Dataset.csv
├── Real_Estate_Property_Analytics_Dashboard.pbix
├── README.md
│
├── Dataset/
│   └── Real_Estate_Property_Dataset.csv
│
├── Dashboard/
│   └── Real_Estate_Property_Analytics_Dashboard.pbix
│
├── Images/
│   └── Real_Estate_Property_Dashboard.png
│
└── LICENSE
💡 Key Insights
Identified differences in property prices across cities.
Compared average property prices across localities.
Identified high-value and affordable property locations.
Analyzed the relationship between property size and price.
Compared prices based on bedrooms and bathrooms.
Analyzed property type distribution.
Compared furnished, semi-furnished, and unfurnished properties.
Analyzed parking, lift, balcony, and garden availability.
Studied property construction and renovation years.
Used geographic visualization to understand city-level price patterns.
📚 Skills Demonstrated
Data Cleaning
Data Transformation
Exploratory Data Analysis
Data Modeling
DAX
Power Query
Power BI
KPI Development
Dashboard Design
Data Visualization
Geographic Data Analysis
Business Intelligence
Business Analysis
🧠 Key Learnings
Built an end-to-end Power BI dashboard from raw real estate data.
Applied Power Query for data cleaning and transformation.
Performed exploratory data analysis to identify pricing patterns.
Designed dynamic KPI cards and interactive visualizations.
Created DAX measures for property analysis.
Used maps for geographic property analysis.
Used slicers to enable interactive data exploration.
Improved dashboard design and data storytelling skills.
Learned how to convert raw property data into actionable business insights.
📌 Dashboard Insights
Property Price Analysis
Analyzed average, minimum, and maximum property prices.

City & Locality Analysis
Compared property prices across cities and localities.

Property Type Analysis
Identified the distribution of different property types.

Property Size Analysis
Analyzed the relationship between living area and property price.

Bedroom & Bathroom Analysis
Compared property prices based on bedrooms and bathrooms.

Amenities Analysis
Analyzed parking, lift, balcony, and garden availability.

Furnishing Analysis
Compared prices across different furnishing categories.

✅ Advantages
Provides a centralized view of real estate property performance.
Tracks important property KPIs in one dashboard.
Helps compare property prices across cities and localities.
Identifies high-value and affordable locations.
Provides interactive filtering through slicers.
Helps analyze property characteristics such as bedrooms and bathrooms.
Shows the relationship between property size and price.
Provides city-level geographic analysis.
Helps analyze furnishing and property amenities.
Reduces manual reporting through automated Power BI calculations.
Makes complex property data easier to understand.
Supports data-driven decision-making.
Demonstrates practical Power BI, DAX, and Power Query skills.
Suitable for portfolio, resume, and business intelligence projects.
❌ Disadvantages
Dashboard insights depend on the accuracy of the source data.
Static datasets do not provide real-time property market information.
Manual data refresh may be required when new data is added.
Limited scalability with extremely large datasets.
Requires basic Power BI knowledge to modify the dashboard.
Does not provide exact property locations without latitude and longitude.
Does not include property photographs or detailed descriptions.
Does not include all external factors that influence property prices.
Does not provide advanced predictive analytics.
Does not integrate with live real estate APIs.
🎁 Benefits of the Real Estate Dashboard
Provides a clear overview of the property market.
Helps compare property prices across different locations.
Identifies expensive and affordable localities.
Helps understand property pricing patterns.
Supports property investment analysis.
Allows quick analysis using interactive filters.
Saves time by presenting multiple analyses in one dashboard.
Helps users understand property characteristics.
Supports data-driven decision-making.
Provides easy-to-understand charts and KPIs.
Improves data storytelling and business reporting.
Can be updated with additional property records.
Demonstrates practical Data Analyst and Power BI skills.
⚠️ Limitations of the Real Estate Dashboard
Does not provide real-time property prices unless connected to a live data source.
Requires regular data refresh when new property data becomes available.
Dashboard performance may decrease with extremely large datasets.
Results depend on the quality and completeness of the source dataset.
Does not predict future property prices.
Does not provide exact property-level map locations without latitude and longitude.
Does not include all economic factors affecting property prices.
Historical property prices may not represent current market conditions.
Limited to the cities and localities available in the dataset.
Does not replace professional real estate valuation or investment advice.
📌 Scope and Limitations
This dashboard is designed to analyze historical real estate property data and present key insights through interactive charts, KPIs, maps, and slicers.

It helps users analyze:

Property prices
Cities
Localities
Property types
Property sizes
Bedrooms
Bathrooms
Furnishing
Amenities
Construction information
However, the dashboard has some limitations. It does not provide real-time property market monitoring, does not predict future property prices, and does not replace professional property valuation systems.

The analysis depends on the accuracy and completeness of the source dataset. The dashboard is intended for data analysis, reporting, visualization, and educational/portfolio purposes.

🚀 Future Enhancements
Integrate real-time real estate APIs.
Add latitude and longitude.
Create exact property-level maps.
Build a machine learning property price prediction model.
Add property price forecasting.
Create investment opportunity scores.
Add automated data refresh.
Publish the dashboard to Power BI Service.
Build a property recommendation system.
Add market trend analysis.
Add neighborhood scoring.
Add price-per-square-foot analysis.
🏢 Business Use Cases
This dashboard can be useful for:

🏠 Property Buyers
💰 Property Investors
🏢 Real Estate Agencies
🏗️ Real Estate Developers
📊 Real Estate Analysts
📈 Market Research Teams
🏦 Financial Institutions
💼 Investment Companies
👨‍💻 Author
Dashrath Landge

Aspiring Data Analyst

Skills
Power BI
SQL
Python
Excel
Pandas
NumPy
Data Analytics
Data Visualization
DAX
Power Query
