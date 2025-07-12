# 🏘️ HDB Resale Flat Analytics Dashboard – Real Estate Capstone Project

This project is part of the Xaltius Academy Data Science Certification Internship. The goal was to build a descriptive analytics dashboard using **Power BI** to analyze Singapore's HDB resale flat market. The dashboard reveals pricing patterns, trends by town and flat type, and property insights to support decision-making.

---

## 🎯 Objectives

- Analyze and visualize HDB resale transactions across Singapore
- Identify price trends by **town**, **flat type**, **floor area**, and **year**
- Create a clean and interactive Power BI dashboard for stakeholder use
- Provide business recommendations backed by data

---

## 📊 Dataset Overview

- **Source**: Singapore HDB Resale Flat data
- **Records**: 141,668 rows
- **Features**: `Month`, `Town`, `Flat Type`, `Floor Area`, `Resale Price`, `Lease Commence Date`, etc.
- **New Feature**: `Price Per Sqm = Resale Price / Floor Area (Sqm)`
- **Engineered Feature**: `Remaining Lease` imputed as `99 - (Year - Lease Commence Date)`

---

## 🧹 Data Cleaning & Preparation

- Renamed all column headers for readability (capitalized, removed underscores)
- Converted 'Month' to datetime and extracted 'Year'
- Derived key pricing and lease duration features
- Imputed missing values for 'Remaining Lease'
- Dropped non-essential columns to streamline visuals

---

## 📈 Dashboard Components

### 📌 Market Overview
- Total Transactions, Avg Resale Price, Avg Price/Sqm (KPI cards)
- Town vs. Avg Resale Price (bar chart)
- Map view of Avg Price by Town (filled map)

### 📌 Price Trends
- Yearly trend of Avg Resale Prices (line chart)
- Avg Resale Price by Flat Type per Year (stacked column chart)

### 📌 Property Insights
- Flat Model vs. Avg Resale Price (treemap)
- Flat Type vs. Floor Area with Price as tooltip (scatter plot)
- Price changes by Flat Type across Years (ribbon chart)

### 📌 Activity Heatmap
- Town-level price heatmap with transaction volume
- Top 10 towns by sales volume
- Table view: Town | Avg Price | Transactions

---

## ⚙️ Interactivity & UX Features

- Sync slicers across pages (Town, Flat Type, Year)
- Enhanced tooltips (e.g., Price per Sqm)
- Custom themes and labels
- Dynamic sorting and drill-through capabilities

---

## 📌 Conclusions & Recommendations

- Clear pricing trends emerge by town and flat type
- `Price per Sqm` is more reliable for comparing value across unit sizes
- Data imputation helps preserve valuable rows
- Recommend combining both raw price and price per sqm for decision-making

### 🧭 Future Scope
- Predictive modeling: use ML to forecast resale prices
- Time series forecasting of transaction volumes by town
- Add geospatial data: MRT proximity, schools, amenities

---

## 🧰 Tools Used

- Power BI for data visualization and dashboard development  
- Excel for initial data wrangling and calculations  
- DAX for calculated columns and KPIs  

---

## 📁 Files Included

- `hdb_resale_dashboard.pbix` – Power BI report file  
- `Manalo_CAPSTONE2 - Real Estate Dataset.pdf` – Project presentation  
- `real_estate_cleaned.xlsx` – Cleaned dataset  
- `README.md` – This documentation  

---

## 📫 Contact

**Fides Angelene R. Manalo**  
📧 fidesangelenemanalo@gmail.com  
🔗 https://www.linkedin.com/in/fides-angelene-manalo-da/
