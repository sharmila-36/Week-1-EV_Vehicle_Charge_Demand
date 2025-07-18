# 🚗 EV Adoption Forecasting

This project focuses on forecasting the adoption trends of Electric Vehicles (EVs) using historical vehicle registration data across various U.S. counties. Understanding these trends helps urban planners anticipate the need for EV charging infrastructure and supports sustainability initiatives.

---

## 📊 Dataset Overview

- **Rows:** 20,819  
- **Columns:** 10  
- **Source Fields Include:**
  - `Date` – Registration date (monthly)
  - `County`, `State` – Location information
  - `Vehicle Primary Use` – e.g., Passenger or Truck
  - `Battery Electric Vehicles (BEVs)` – Fully electric vehicle count
  - `Plug-In Hybrid Electric Vehicles (PHEVs)` – Hybrid vehicle count
  - `Electric Vehicle (EV) Total` – BEVs + PHEVs
  - `Non-Electric Vehicle Total` – Traditional vehicles
  - `Total Vehicles` – Sum of EV and non-EV
  - `Percent Electric Vehicles` – EV share among all vehicles

---

## 🛠️ What’s Done

- Converted `Date` column to proper datetime format
- Filled missing values in `County` and `State` using `"Unknown"`
- Identified and capped outliers in `Percent Electric Vehicles` using IQR bounds
- Ensured clean and structured data for further modeling

---

## 📁 Files

- `ev_forecasting.ipynb` – Contains code for:
  - Data loading
  - Preprocessing
  - Outlier treatment
  - Initial exploration

---

## ✅ Planned Improvements

- Build regression models (e.g., Random Forest, Linear Regression)
- Forecast future EV adoption
- Visualize trends across time and regions

---
