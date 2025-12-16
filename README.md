# 🚖 Pathao Ride-Sharing Analytics Dashboard (Power BI)

## 📘 Overview  
This project presents an end-to-end data analytics solution for a **simulated Bangladeshi ride-sharing company — Pathao**.  
The goal was to analyze **platform performance, driver operations, and customer behavior** to uncover insights that support business growth and operational efficiency.

All datasets were **synthetically generated** using Python’s Faker library with Bangladesh-style names and locations to closely reflect realistic ride-sharing patterns in Dhaka and surrounding regions.

The interactive **Power BI dashboard** visualizes:  
- Business performance (YoY & MoM trends)  
- Driver attrition & operational pressure  
- Loyalty, churn, and retention metrics  
- Revenue distribution & customer segmentation  

⚔️ Live Dashboard: [Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTU5ZTcwMGYtNjY2Ni00M2Q4LTlkMzQtNzliYzAwNzBlM2Y2IiwidCI6IjZjMWYxNzUyLTU1NmQtNDhjNC1hNmFlLWQ2NTA5MDU2MmVkNCIsImMiOjEwfQ%3D%3D)

---

## 📊 Dataset Summary

| Dataset            | Description                                          | Rows  | Key Columns                                                                 |
|-------------------|------------------------------------------------------|-------|-----------------------------------------------------------------------------|
| **Rides.csv**     | Ride transactions (2023–2024)                        | 17,000 | RideID, PassengerUserID, DriverID, StartDate, EndDate, Fare, DistanceKM, DurationMin, Status |
| **Drivers.csv**   | Registered driver information                         | 47    | DriverID, Name, Gender (all Male), JoinDate, Status                         |
| **Vehicles.csv**  | Vehicle data linked to drivers                        | 47    | VehicleID, DriverID, Type, Model, RegistrationNo, Status                    |
| **Passengers.csv**| Passenger demographic and account profiles            | 1,200 | PassengerUserID, Name, Gender, JoinDate, Region                             |
| **Date_Table.csv**| Custom date dimension                                 | 730   | Date, Year, Month, Quarter, Weekday                                         |

### 🔗 Data Source
All datasets were generated using **Python + Faker + ChatGPT-assisted logic**.  
No real company or customer information was used.

---

## 💡 Key Insights

### 1️⃣ Business Overview (Executive Summary)

- **📈 Ride Volume Growth:**  
  ~25% increase in total rides in 2024 vs 2023.
  
- **💰 Revenue Growth:**  
  Higher average fare per ride → increased commission earnings.

- **🗺️ Dhaka Leads the Market:**  
  60%+ of total rides come from Dhaka district.

- **❌ Cancellation Trends:**  
  Driver cancellation + accident-related cancellation ≈ **18% of all rides**.

---

### 2️⃣ Driver Operations

- **👨‍✈️ Driver Attrition:**  
  Active driver rate dropped from **~96% (2023)** to **~65% (2024)**.
  
- **⏳ Impact on Passengers:**  
  Wait time increased from **4 min → 7 min** due to driver shortage.

- **⛽ Imbalanced Performance:**  
  A small group of drivers completes most rides → incentive optimization needed.

- **🧭 Vehicle Utilization:**  
  Several vehicles remained underutilized due to inactive drivers.

---

### 3️⃣ Customer Analytics

- **💎 Loyal Passengers:**  
  ~18% consistently ride **5+ times in consecutive months**.

- **🚶‍♂️ Churned Passengers:**  
  ~28% have not ridden in the last **3 months**.

- **💵 Revenue Concentration:**  
  The **top 10%** passengers contribute **45%+** of total revenue.

- **⭐ Ratings:**  
  Average rider experience rating is **4.5 / 5**.

---

## 🧰 Tools & Technologies

| Category           | Tools                                   |
|--------------------|------------------------------------------|
| Data Generation    | Python, Faker                            |
| Data Processing    | Pandas, NumPy                            |
| BI & Visualization | Power BI                                 |
| Data Modeling      | DAX, Star Schema (Fact + Dimensions)     |
| Version Control    | Git, GitHub                              |

---

## 📈 Dashboard Pages

### **1️⃣ Business Overview**
- KPI cards  
- YoY & MoM trend lines  
- Ride distribution map  
- Cancellation analysis donut chart  

### **2️⃣ Driver Analytics**
- Attrition vs active driver trends  
- Driver engagement analysis  
- Wait time & demand relationship  
- Vehicle utilization metrics  

### **3️⃣ Customer Insights**
- Loyalty & churn modeling  
- Month-to-month retention funnel  
- RFM segmentation  
- Revenue Pareto (Top 10% customers)  

---

## 🧠 Key Learnings

- Designed a **complete BI pipeline** with synthetic but realistic data.
- Developed DAX formulas for:  
  - churn rate  
  - loyalty %  
  - YoY / MoM growth  
  - revenue segmentation  
- Built a multi-page dashboard aligned with **real-world ride-sharing KPIs**.
- Strengthened experience in **data modeling, ETL, visualization, and storytelling**.

---


