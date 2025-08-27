# ESG-Financial-Risk-Detection-for-Strategic-Decision-Making

# 🌍 ESG–Financial Risk Dashboard (2015–2025)

## 📌 Project Overview
This dashboard provides a **strategic overview of ESG (Environmental, Social, Governance) performance and financial risks** across global industries between 2015–2025.  
It helps executives, analysts, and stakeholders quickly identify **high-risk companies, industry performance, and sustainability trade-offs** between profit and environment.  

---

## ⚡ Key Features
- **One-Page Dashboard Layout** for quick executive decision-making  
- **KPI Cards**: ESG Overall, Profit Margin, Revenue, and Company Count  
- **Trends Over Time**: ESG score progression by industry and year  
- **Risk Analysis**: ESG vs Profit Margin scatter plot with Risk Level classification  
- **Finance vs Environment**: Combo chart comparing Revenue and Carbon Emissions  
- **Industry Breakdown**: Revenue share and performance by sector  
- **Company-Level Table**: Quick reference of ESG score, Profit Margin, and Revenue  

---

## 📊 Dataset Details
The dataset is **simulated for learning** but designed to reflect real-world ESG & financial reporting structures.  

**Columns included:**  
- `CompanyID` – Unique company identifier  
- `CompanyName` – Name of company  
- `Industry` – Sector/industry classification  
- `Region` – Geographic region  
- `Year` – Year of record (2015–2025)  
- `Revenue` – Total revenue (in millions)  
- `ProfitMargin` – Net profit margin %  
- `MarketCap` – Market capitalization (in millions)  
- `GrowthRate` – Year-over-year growth %  
- `ESG_Overall` – Combined ESG score  
- `ESG_Environmental` – Environmental score  
- `ESG_Social` – Social score  
- `ESG_Governance` – Governance score  
- `CarbonEmissions` – Carbon emissions (in tons)  
- `WaterUsage` – Water usage (liters)  
- `EnergyConsumption` – Energy usage (kWh)  

---

## 🛠️ Tools & Tech
- **Power BI** (DAX, Power Query, Visualization)  
- **Excel/CSV** for dataset preparation  
- **DAX Measures** for KPIs & Risk Level calculation  

---

## 🔑 DAX Measures Used
```DAX
Avg ESG Overall = AVERAGE('Table'[ESG_Overall])
Avg Profit Margin % = AVERAGE('Table'[ProfitMargin])
Total Revenue = SUM('Table'[Revenue])
Total Market Cap = SUM('Table'[MarketCap])

Risk Level = 
SWITCH(
    TRUE(),
    'Table'[ESG_Overall] < 40, "High Risk",
    'Table'[ESG_Overall] >= 40 && 'Table'[ESG_Overall] < 70, "Medium Risk",
    'Table'[ESG_Overall] >= 70, "Low Risk",
    "Unknown"
)

Carbon per Revenue = 
DIVIDE(SUM('Table'[CarbonEmissions]), SUM('Table'[Revenue]))

---
