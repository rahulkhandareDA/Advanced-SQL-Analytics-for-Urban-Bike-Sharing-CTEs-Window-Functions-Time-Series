# Advanced SQL Analytics for Urban Bike-Sharing: CTEs, Window Functions & Time Series



## Project Background

UrbanRoll is an urban bike-sharing platform designed for short-distance commuting and casual city travel. The platform operates in a high-frequency mobility environment where growth, retention, and operational efficiency are tightly coupled with user behavior and station availability.

This project applies SQL-based analytics to ride, user, and station data to answer key business and operational questions faced by shared mobility platforms.

---

## Analysis Framework

Each section follows a structured analytics flow:

**Business Question → Insight → Recommendation → Visual → SQL Query**

---

## 1️⃣ Membership-Based Usage Analysis

### Business Question  
How do different membership types use the UrbanRoll platform?

### Key Insight  
Subscriber users generate the majority of ride volume with shorter, more consistent trips, while casual users take longer and more irregular rides.

### Recommendation  
Design engagement and pricing strategies separately for subscribers and casual users instead of applying uniform policies.

### Supporting Visual  
- Bar chart: Total rides by membership  
- Line or box plot: Average ride duration by membership  

### SQL Query Reference  
`membership_usage_analysis.sql`

---

## 2️⃣ Time-Based Demand & Peak Hour Analysis

### Business Question  
When does demand peak during the day?

### Key Insight  
Ride volume follows a strong commuter-driven pattern with distinct peak hours and low midday activity.

### Recommendation  
Align operational planning and bike availability with observed peak demand windows.

### Supporting Visual  
- Hourly ride volume bar chart  

### SQL Query Reference  
`peak_hour_analysis.sql`

---

## 3️⃣ Daily Demand Trend (7-Day Moving Average)

### Business Question  
Is platform usage growing consistently over time?

### Key Insight  
Daily ride counts show volatility, but the 7-day moving average reveals a stable underlying growth trend.

### Recommendation  
Use smoothed trends rather than raw daily metrics for performance monitoring and forecasting.

### Supporting Visual  
- Line chart: Daily rides vs 7-day moving average  

### SQL Query Reference  
`daily_moving_average.sql`

---

## 4️⃣ Station Popularity & Utilization

### Business Question  
Which stations experience the highest ride activity?

### Key Insight  
A small subset of stations accounts for a disproportionate share of total ride starts.

### Recommendation  
Prioritize maintenance, capacity, and availability at high-traffic stations.

### Supporting Visual  
- Top 10 stations by ride volume  

### SQL Query Reference  
`station_popularity.sql`

---

## 5️⃣ Ride Duration Segmentation

### Business Question  
How are rides distributed by duration?

### Key Insight  
Rides naturally cluster into short, medium, and long duration segments, reflecting commuter and leisure usage patterns.

### Recommendation  
Use duration segments to inform pass design and pricing thresholds.

### Supporting Visual  
- Ride distribution by duration category  

### SQL Query Reference  
`ride_duration_segmentation.sql`

---

## 6️⃣ Station-Level Net Ride Flow (Rebalancing Analysis)

### Business Question  
Which stations consistently gain or lose bikes?

### Key Insight  
Certain stations act as persistent bike sinks or sources, indicating rebalancing inefficiencies.

### Recommendation  
Implement targeted rebalancing and incentive mechanisms to correct station-level imbalances.

### Supporting Visual  
- Net ride flow table or bar chart  

### SQL Query Reference  
`net_ride_flow.sql`

---

## 7️⃣ Growth & Churn Proxy Analysis

### Business Question  
Is user growth sustainable when accounting for churn?

### Key Insight  
MoM user growth alone overstates platform health; inactivity-based churn provides essential retention context.

### Recommendation  
Track net user growth by combining acquisition and churn metrics.

### Supporting Visual  
- MoM growth vs churn trend  

### SQL Query Reference  
`mom_growth_and_churn.sql`

---

## Conclusion

This project demonstrates a structured SQL-driven approach to answering real-world business and operational questions in a shared mobility context.

By linking business questions directly to insights, recommendations, and supporting SQL queries, the analysis reflects how data teams communicate findings to decision-makers in production environments.

---

# Skills: SQL, MySQL, Business Intelligence, Data Analysis, CTEs, Window Functions, Time-Series Analysis
