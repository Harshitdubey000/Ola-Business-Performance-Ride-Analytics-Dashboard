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
<img width="1165" height="740" alt="Screenshot 2025-12-14 170035" src="https://github.com/user-attachments/assets/e3520602-6f93-4b03-907c-ce84a955ef89" />


| Payment Insights |
|---------------|
<img width="1162" height="723" alt="Screenshot 2025-12-14 170100" src="https://github.com/user-attachments/assets/d264ba35-433f-4e9b-9936-5b9d1082e2a9" />



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
