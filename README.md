# 📊 Ola-Business-Performance-Ride-Analytics-Power BI Dashboard


## 📌 Project Overview
This project is an **end-to-end data analytics dashboard** built using **Power BI**, focused on analyzing Ola ride booking data.  
The dashboard provides actionable insights into booking trends, revenue, ride status, customer behavior, and performance metrics to support data-driven decision making.

---

## 🛠 Tools & Technologies Used
- **Power BI** – Data visualization & dashboard creation  
- **Microsoft Excel** – Raw data source  
- **Power Query** – Data cleaning & transformation  
- **DAX** – Calculated measures and KPIs  

---

## 📂 Dataset Details
- **File Name:** `Bookings-100000-Rows.xlsx`
- **Records:** 100,000+ ride bookings
- **Key Columns:**
  - Booking Date
  - Ride Status (Completed / Cancelled)
  - Vehicle Type
  - Payment Method
  - Trip Distance
  - Fare Amount
  - Customer & Driver details

---

## 📈 Key Insights from Dashboard
- Total bookings, completed rides, and cancellation rate
- Revenue trends by date and vehicle type
- Popular payment methods used by customers
- Ride demand analysis over time
- Performance comparison across vehicle categories

## 📸 Dashboard Preview

| Overview |
|---------|
| ![]("C:\Users\harsh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-14 170035.png") | ![]("C:\Users\harsh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-14 170100.png") |

| Payment Insights |
|---------------|
![]("C:\Users\harsh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-14 170100.png") |


---

## 📊 Dashboard Features
- Interactive slicers (Date, Vehicle Type, Payment Mode)
- KPI cards for quick performance overview
- Trend analysis using line & bar charts
- Clean, user-friendly layout for business stakeholders

---

## 🧮 Key Measures (DAX Examples)
```DAX
Total Bookings = COUNT(Bookings[Booking ID])

Total Revenue = SUM(Bookings[Fare Amount])

Completed Rides = 
CALCULATE(
    COUNT(Bookings[Booking ID]),
    Bookings[Ride Status] = "Completed"
)
