# Logistics-Operation-Analysis
Power BI + Power Query
# Project Overview
This project is an end-to-end logistics operations analysis built using Power BI and Power Query. It analyzes real-world logistics data covering trips, delivery events, drivers, routes and facilities to uncover key operational insights related to delivery performance, detention patterns and delay trends.
# Objectives
- Analyze on-time pickup and delivery performance across routes and drivers
- Identify detention hotspots by location and facility
- Discover correlation between pickup delays and detention duration
- Track delay trends by day of week and route
- Build an interactive dashboard to support operational decision-making
# Dataset
- Source: logistics operations dataset
- Contains information on trips, delivery events, drivers, routes, trucks, fuel and maintenance
- Data covers 85,410+ trips across multiple cities, drivers and facility locations
- Includes scheduled vs actual timestamps, detention duration and on-time flags
# Tools & Techniques
- Power BI (Data visualization and interactive dashboard creation)
- Power Query (Data cleaning and transformation)
- DAX (KPI measures and calculated columns)
- Data Modeling (Star schema with relationships across 7 tables)
# Data Preparation
- Loaded and connected 7 related tables in Power BI data model
- Built star schema with Trips and Delivery Events as core fact tables
- Created relationships across Drivers, Routes, Facilities, Trucks and Loads tables
- Engineered calculated columns including Delay Minutes and Day of Week
- Filtered terminated drivers to ensure active-only performance analysis
- Validated on-time flag data types and corrected filter logic in DAX
# Dashboard Features
## KPIs
- Total Trips
- On Time Pickup Rate
- On Time Delivery Rate
- Detention Rate
- Avg Pickup Delay (mins)
- Avg Delivery Delay (mins)
- Avg Detention Duration (mins)
- Total Detention Hours
# Visualizations
- On Time Delivery Rate by Route (clustered bar chart)
- Driver Performance Matrix with conditional formatting
- On Time Delivery Trend Over Time (line chart)
- Top 10 Locations by Total Detention Hours (bar chart)
- Pickup Delay vs Detention Duration (scatter plot)
- Detention Hotspots by Location (bubble map)
- Average Delay by Day of Week (bar chart)
# Interactive Filters & Slicers
- Year filter
- City filter
- Driver filter
- Slicers synced across both dashboard pages
# Key Insights
- Only 44.62% of trips were delivered on time despite a 66.73% on-time pickup rate, revealing delays compound significantly during transit
- 86.86% of all trips incurred detention averaging 92 minutes, indicating detention is a systemic operational issue not an exception
- Average pickup delay of 119 minutes cascades into average delivery delays of 180 minutes, confirming a strong compounding effect
- Kansas City recorded the highest total detention hours among all facility locations, making it a priority for operational intervention
- Wednesday recorded peak average delays, suggesting mid-week scheduling or capacity pressure points
# Recommendations
- Prioritize on-time pickup compliance as the primary lever to reduce downstream delivery delays
- Investigate Kansas City facility operations for structural causes of high detention
- Review mid-week driver scheduling and route allocation to address peak delay patterns
- Set detention threshold alerts for facilities consistently exceeding average duration
- Consider driver-level coaching for those with below-average OTD rates and above-average detention times
# Conclusion
This analysis reveals that logistics delays are not isolated events but systemic patterns rooted in pickup punctuality and facility-level bottlenecks. By addressing on-time pickup compliance and targeting high-detention locations, operations teams can significantly reduce detention costs and improve overall delivery performance.
## Files Included
- Logistics Operation Data Analysis.pbix
- Overview & Performance Dashboard Screenshot
- Delay & Detention Dashboard Screenshot
- Key Insights Screenshot
# Future Improvements
- Incorporate fuel cost and maintenance data into performance scoring
- Add predictive delay analysis using historical patterns
- Expand driver performance benchmarking with monthly metrics
