🚖 OLA Data Analyst Project
This project is a data analysis case study focused on Ola ride bookings. It involves data cleaning, SQL queries, and Power BI dashboards to gain insights into ride patterns, cancellations, revenue, and ratings.

📂 Project Overview
Dataset: Simulated ride booking data for Bengaluru.
Tools Used: SQL, Power BI, Python (optional for data manipulation).
Key Focus Areas:
Booking trends over time
Cancellation patterns
Customer & driver ratings analysis
Revenue insights
Ride distance distribution
🛠️ Data Columns
The dataset includes:

Ride Details: Booking ID, Date, Time, Vehicle Type, Pickup & Drop Locations
Performance Metrics: VTAT (Vehicle Time to Arrive), CTAT (Customer Time to Arrive)
Cancellations & Incomplete Rides: Reasons for cancellations (Customer/Driver), Incomplete rides
Financial & Ratings: Booking Value, Payment Method, Customer & Driver Ratings
🔍 SQL Queries
Example queries used in this project:
1️⃣ Retrieve all successful bookings:

sql
Copy
Edit
SELECT * FROM bookings WHERE Booking_Status = 'Success';  
2️⃣ Find the average ride distance per vehicle type:

sql
Copy
Edit
SELECT Vehicle_Type, AVG(Ride_Distance) AS avg_distance FROM bookings GROUP BY Vehicle_Type;  
3️⃣ Get the top 5 customers by the number of rides booked:

sql
Copy
Edit
SELECT Customer_ID, COUNT(Booking_ID) AS total_rides FROM bookings  
GROUP BY Customer_ID ORDER BY total_rides DESC LIMIT 5;  
📊 Power BI Dashboards
The project includes interactive Power BI reports covering:

📈 Ride Volume Over Time
🚗 Top Vehicle Types by Distance
📊 Booking Status Breakdown
💰 Revenue by Payment Method
⭐ Customer vs. Driver Ratings
