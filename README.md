# 🚗 EV Adoption Forecasting

This project aims to **forecast the future adoption of Electric Vehicles (EVs)** using historical vehicle registration data from Washington State. With the growing push for sustainable transport, forecasting EV growth is crucial for **urban planning and infrastructure development**, especially for EV charging stations.

---

## 📊 Dataset

- **Source**: [Kaggle - EV Population Size 2024](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024/data)
- **Features include**:
  - `Date`, `County`, `State`
  - `Vehicle Primary Use` (Passenger/Truck)
  - `Battery Electric Vehicles (BEVs)`
  - `Plug-In Hybrid Electric Vehicles (PHEVs)`
  - `Non-Electric Vehicle Total`
  - `Percent Electric Vehicles`

---

## 🛠️ What’s Done

- Converted `Date` column to datetime format
- Filled missing values in `County` and `State` with `'Unknown'`
- Removed invalid or null entries
- Capped outliers in `Percent Electric Vehicles` using the IQR method
- Prepared the dataset for regression modeling

---

## 📁 Files

- `ev_forecasting.ipynb` – Jupyter Notebook containing data exploration, cleaning, and preprocessing steps.

---

## ✅ Future Improvements

- Build and evaluate a regression model for EV adoption forecasting
- Visualize predictions and trends across counties and time
- Optimize feature engineering for better model performance
