# Hotel-Revenue-Analysis
# Project Overview: 
The hotel revenue dashboard is designed to provide a comprehensive view of the hotel's revenue performance for Luxury and Business Hotel category. The dashboard will be built using Power BI.
# AIM:
To know reasons for Losing market share and Revenue in Luxury & Business hotel category.
# Insights:
1. **Dynamic Pricing** - One important insight for improving hotel revenue is implementing dynamic pricing strategies. This involves changing hotel prices in real-time based on factors such as demand, seasonality, and competitor pricing. By adjusting prices according to market conditions, hotels can maximize their revenue and improve occupancy rates.
2. **Locations** - The location of a hotel can play a significant role in its pricing. Hotels located in popular tourist destinations or business districts tend to charge higher prices than those located in less popular areas.
3. **Room Type** - The type of room also impacts hotel prices. For example, suites or rooms with a view tend to be more expensive than standard rooms.
4. **Customer Reviews** - Customer reviews and ratings can provide valuable insights into the quality of a hotel and its pricing. Analysing reviews can help identify areas where hotels may need to improve to justify their pricing.
5. **Direct Booking** - Direct booking allows hotels to bypass third-party booking platforms, and save on commission fees. By offering incentives such as lower prices, room upgrades or loyalty rewards, hotels can encourage customers to book directly with them and improve revenue.
# Data Sources:
Data are in the form of excel files.
# Data Model:
The data model will include tables for room occupancy, room type, revenue, Booking Status, Hotel category, City, booking_ID, Booking platforms, Booking status, Dates like check_in_date, Check_out_date etc.
The tables will be linked together through common fields, such as -
| table1   | table2                | connected columns       |
| -------- | --------------------- | ----------------------- |
| DimDate  | FactAggregatedBooking | Check_in_date           |
| DimHotel | FactAggregatedBooking | property_id             |
| DimHotel | FactBooking           | property_id             |
| DimDate  | FactBooking           | Check_in_date           |
| DimRooms | FactAggregatedBooking | room_id & room_category |
| DimRooms | FactBooking           | room_id & room_category                        |

# Visualization:
The dashboard will include several visualizations, including line charts, bar charts, donut chart and tables, to display revenue performance over time, by revenue stream, and by room occupancy, Average User ratings and many more.
![image](https://user-images.githubusercontent.com/111041023/230767964-1dad453a-6df8-4c2d-9d58-89beedd88c67.png)

# Layout: 
The layout of the dashboard will be designed to be easy to navigate and visually appealing. *Filters* will be prominently displayed at the top of the dashboard. *Key metrices* are place in the top right of the visuals.

---
# Key metrics for analysing revenue in Hotel Industry:
1. **Occupancy Rate** - Occupancy rate measures the percentage of available rooms that are occupied over a given period. A higher occupancy rate indicates better utilization of resources and higher revenue.
2. **Average Daily Rage (ADR)** - ADR measures the average rate charged per occupied room per day. By tracking ADR, hotels can identify pricing trends and adjust pricing strategies to maximize revenue.
3. **Revenue Per Available Rooms (RevPAR)** - RevPAR measures the total revenue generated per available room over a given period. By analysing RevPAR, hotels can understand how effectively they are monetizing their available rooms and identify areas for improvement.
4. **Daily Sale Revenue Per Available Room (DSRN)** - A metric that measures the total revenue generated per available room per day. It is calculated by dividing the total revenue generated from all sources (including room revenue, food and beverage sales, and other ancillary services) by the total number of available rooms over a given period.
5. **Difference between ADR and DSRN** - The key difference between **ADR** and **DSRN** is that *ADR only considers room revenue*, while *DSRN includes revenue from all sources.* ADR provides insights into pricing strategies and the revenue generated per guest, while DSRN provides a more comprehensive view of the hotel's overall revenue generation.
6. **Realization** - Realization refers to the percentage of a hotel's total available revenue that is actually collected or realized. It measures how effectively the hotel is converting potential revenue into actual revenue.
   *Realization = Actual Revenue / Total Available Revenue*
   For example, let's say a hotel has total available revenue of $100,000 for a given period, but only collects $80,000 of that revenue. The realization for that period would be: 
   Realization = $80,000 / $100,000 = 0.8 or 80%
   
   ### Q. If I have a total of 100 bookings, but 10 were cancelled and 5 were no-shows, how do I calculate the realization?
   **Realization = Actual Revenue / Potential Revenue**
   *Actual Revenue* = Revenue generated from completed bookings. 
   *Potential Revenue* = Total revenue that could have been generated if all bookings were completed as planned.
   
   potential booking = 100
   actual booking = 85.
   Actual Revenue = 8500$ (suppose)
   *ADR* = 8500/85 = 100
   *potential revenue* = 100(rooms) * 100(ADR)
   **Realization** = 8500/10000 = 85% 
