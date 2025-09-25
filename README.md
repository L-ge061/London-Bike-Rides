# London Bike Sharing Analysis
Dataset Source: https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset


## Overview
This project will explore the **London Bike Sharing Dataset** (Kaggle) to understand demand patterns and external factors affecting bike usage.  
The workflow combines **Python (data cleaning & preparation)** and **Tableau (interactive dashboard)** to uncover trends in seasonality, weather impact, and rider behavior.  

---

## Problem Statement
Bike sharing systems provide an eco-friendly and efficient transportation alternative in major cities.  
However, **demand for shared bikes fluctuates heavily** depending on factors such as **weather, season, temperature, and time of day**.  
The challenge is to understand:
- When and why ridership increases or decreases.  
- How external factors (weather, seasonality) affect demand.  
- What insights operators can use to improve **bike availability, maintenance scheduling, and customer satisfaction**.  

This project aims to analyze and visualize the **London Bike Sharing Dataset** to uncover patterns and trends that can guide better operational and strategic decisions.

---

## Data Preparation (Python)
Steps completed in Jupyter Notebook:
- Imported the dataset and checked for missing or inconsistent values.  
- Renamed columns into more descriptive names (e.g., `cnt` → `count`).  
- Scaled humidity to proper decimal values.  
- Mapped **season codes** (0–3) to `spring, summer, fall, winter`.  
- Mapped **weather codes** (1, 2, 3, etc.) to `Clear, Clouds, Rain, Snowfall, etc`.  
- Exported the cleaned dataset into Excel for visualization.  

---

## Dashboard (Tableau)
Built an interactive dashboard with the following features:
- **Total Rides**: Shows total number of rides in user selected date ranges.  
- **Moving Average**: Shows seasonal fluctuations and demand trends in user selected date or date ranges.  
- **Temperature vs. Wind Speed Heatmap**: Reveals ride activity under different weather conditions.  
- **Weather & Hourly Trends**: Filters highlight how rides vary by weather type and time of day.

## Screen Shots
<img width="1396" height="799" alt="Screenshot 2025-09-25 at 2 26 47 PM" src="https://github.com/user-attachments/assets/1f806b64-f040-43a5-aaee-81615633847f" />


<img width="1396" height="799" alt="Screenshot 2025-09-25 at 2 27 55 PM" src="https://github.com/user-attachments/assets/56895eb0-c7b4-4c6b-8764-f1f3b1eb42f3" />



## Findings & Insights
- **Seasonality**: Bike demand peaks in **summer** and declines in **winter**, showing a clear annual cycle.  
- **Weather Sensitivity**: Clear or scattered clouds lead to higher ride volumes, while rain and strong winds significantly reduce usage.  
- **Temperature Effect**: Optimal ridership occurs around **10–20°C**, dropping off in colder or hotter conditions.  
- **Commuter Behavior**: Rides spike in the **afternoon and early evening (14:00–19:00)**, aligning with commuting and leisure travel patterns.  
- **Operational Use**: Moving average trends help identify abnormal dips or surges (holidays, extreme weather), useful for resource allocation.  

---

## Business Recommendations
Based on the analysis, here are actionable suggestions for bike-sharing operators in London:
1. **Capacity Planning**  
   - Increase bike availability during **summer months** and in **afternoon/evening hours**.  
   - Ensure rebalancing teams are ready for high-demand commuting zones.

2. **Maintenance Scheduling**  
   - Use **low-demand winter months** for large-scale maintenance and bike replacement.  
   - Schedule routine repairs overnight or early mornings when demand is minimal.

3. **Dynamic Pricing & Incentives**  
   - Offer **discounts or promotions** during winter and rainy days to encourage usage.  
   - Introduce **peak-hour pricing** during summer afternoons to manage demand.

4. **Weather-Based Communication**  
   - Send **real-time alerts** through apps about bike availability during adverse weather.  
   - Recommend alternative routes or incentives when heavy rain/wind is forecast.

5. **Long-Term Strategy**  
   - Align expansion plans with areas showing consistent demand in clear, mild-weather conditions.  
   - Partner with local businesses or transit systems to integrate bike use into broader city mobility plans.  

---

## Conclusion
London’s bike sharing system exhibits strong **seasonal and weather-driven patterns**, with demand highly concentrated during mild, clear-weather days and commuter hours. These insights can inform:  
- **Capacity Planning**: Ensure bike availability during peak summer demand.  
- **Maintenance Scheduling**: Utilize winter’s low usage for repairs.  
- **Policy & Pricing**: Consider promotions or dynamic pricing to encourage winter ridership.  

---

## What’s Next
With more time, further exploration could include:
- **Predictive Modeling**: Use regression or time-series models to forecast demand.  
- **User Segmentation**: Analyze weekday vs. weekend patterns in more detail.  
- **External Data Integration**: Add event data (holidays, public transport strikes) for richer insights.  
- **Geospatial Analysis**: If station-level data is available, map hotspots and optimize bike distribution.  
