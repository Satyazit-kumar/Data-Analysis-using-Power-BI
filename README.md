
# ✈️ Airline Data Management and Analysis using Power BI

## 📌 Project Overview

This project demonstrates how Power BI can be used to analyze and visualize airline operational data to derive actionable insights. The analysis spans flight performance, ticket booking trends, and passenger data to assist airline operators in optimizing operations and improving customer satisfaction.

---

## 🎯 Objective

To perform end-to-end data analysis and build interactive dashboards that provide insights into:
- Flight operations and punctuality
- Passenger distribution
- Ticket booking statuses and cancellation trends

---

## 📁 Datasets Used

- **Flight Information**: FlightID, FlightNumber, Airline, Destination, Status
- **Passenger Information**: PassengerID, FlightID, SeatNumber
- **Ticket Information**: TicketID, FlightID, BookingStatus

---

## ✅ Tasks Performed

### 1. Data Preparation and Cleaning 
- Cleaned datasets in Power Query by:
  - Removing duplicates
  - Eliminating blank rows
  - Formatting columns

### 2. Data Modelling 
- Created appropriate relationships between datasets using `FlightID` as the primary key.
- Configured correct cardinality and referential integrity.

### 3. Enhanced Data Insights 
- Added conditional columns to classify flights as **"Best"** or **"To Be Improved"**
- Used "Column from Examples" to extract flight numbers.

### 4. DAX Calculations 
- Total passengers for Flight 1003  
  `CALCULATE(COUNT(passenger_information[FlightID]), passenger_information[FlightID] = 1003)`
- Total tickets booked  
  `COUNT(ticket_information[TicketID])`
- Table for "Best" flights  
  `FILTER(flight_information, flight_information[Flight Classification] = "Best")`

### 5. Visualizations and Interactive Features 
- Created charts for:
  - Passenger count by airline
  - Ticket booking statuses
  - Flights by airline and destination
- Added:
  - Drillthrough and slicers for airline-specific and destination-based insights
  - Quick views

### 6. Final Dashboard and Power BI Service 
- Published interactive dashboard
- Configured Row-Level Security (RLS) for **Airline A**
- Set up scheduled data refresh at **5 PM daily**

---

## 📊 Key Insights

1. **Airline D** operates the highest number of flights (62).
2. **40%** of flights to Los Angeles and **39%** to Chicago were canceled.
3. **48%** of flights to Houston were delayed.
4. **Airline A and D** have the highest cancellations.
5. **Total Passengers**: 100  
   **Tickets Booked**: 50  
   **Tickets Cancelled**: 19  
   **Total Flights**: 200  
   - On-Time: 82  
   - Delayed: 58  
   - Cancelled: 60

---

## 💡 Recommendations

- Investigate and reduce high delay and cancellation rates to improve customer experience.
- Identify reasons behind cancellations, especially for Airline A and D.
- Analyze delays on the Houston route.
- Optimize flight schedules based on route popularity and occupancy.

---



## 🛠 Tools Used

- Microsoft Power BI
- Power Query Editor
- DAX (Data Analysis Expressions)

---

## 👤 Author

**Satyajit**  
Data Analyst | Power BI Enthusiast

---


This project is part of an academic submission and is for educational purposes only.

