# 🏥 Healthcare Data Analysis Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-00BFFF?style=for-the-badge)
![Rating](https://img.shields.io/badge/Score-8.2%2F10-97C459?style=for-the-badge)

> A real-time, interactive healthcare analytics dashboard built in Microsoft Power BI — covering patient demographics, billing analysis, doctor/hospital performance, and medical condition trends.

---

## 📊 Dashboard Preview

![Healthcare Dashboard](<img width="1201" height="683" alt="Healthcare data analysis" src="https://github.com/user-attachments/assets/2fab490f-af8a-4e1f-8c1f-ef08428d06a3" />
)

---

## 🔍 Overview

This Power BI dashboard provides a comprehensive view of healthcare operations data, enabling stakeholders to monitor key metrics at a glance and drill down by filters like admission type, gender, blood type, age group, and more.

The dashboard was designed to replicate a professional dark-themed analytics layout with neon-style accents, combining both aesthetic appeal and functional data storytelling.

---

## 📌 Key Metrics (KPI Cards)

| Metric | Value |
|---|---|
| Total Billing Amount | $1.42 Billion |
| Average Billing Amount | $25.54K |
| Total Patients | 56K |
| Total Female Patients | 28K |
| Total Male Patients | 22K |
| Non-Binary Patients | 6K |

---

## 📈 Visuals Included

### 1. Total Patients by Test Results — Donut Chart
- Normal: 31K (55%)
- Abnormal: 19K (35%)
- Inconclusive: 6K (10%)

### 2. Total Billing Amount by Month — Line Chart
- Monthly trend from January to December
- Peak billing in August ($123M), lowest in April ($100M)

### 3. Total Billing Amount by Insurance Provider — Treemap
- Medicare: $707.5M
- UnitedHealthCare: $426.1M
- Cigna: $142.8M
- Aetna: $141.1M

### 4. Total Patients & Avg Billing by Medical Condition — Combo Bar Chart
- Conditions: Diabetes, Hypertension, Obesity, Arthritis, Cancer, Asthma
- Dual axis: patient count (bars) + average billing (line overlay)

### 5. Doctors & Hospitals Slicers
- Horizontally scrollable chiclet-style slicers for doctor and hospital selection
- 3D illustrated doctor team image panel
- Real hospital photo panel

---

## 🎛️ Interactive Filters / Slicers

- Admission Type
- Age (bins)
- Blood Type
- Gender
- Room Number
- Patient ID
- Year, Quarter, Weekday (top-right dropdowns)

---

## 🎨 Design System

| Element | Value |
|---|---|
| Background | `#080C1A` (near-black navy) |
| Card background | `#0D1438` |
| Primary accent | `#00BFFF` (cyan) |
| Secondary accent | `#FF4500` (orange-red) |
| Chart line color | `#00BFFF` |
| Text | `#FFFFFF` |
| Border/glow | `#00BFFF` 1–2px |

---

## 🗂️ File Structure

```
healthcare-dashboard/
│
├── HealthcareDashboard.pbix       # Main Power BI file
├── README.md                      # This file
├── dashboard_preview.png          # Dashboard screenshot
└── data/
    └── healthcare_data.csv        # Source dataset (sample)
```

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `HealthcareDashboard.pbix` in **Power BI Desktop** (free download from Microsoft)
3. If prompted, update the data source path to your local `data/` folder
4. Interact with slicers and filters to explore the data
5. To publish: **File → Publish → Publish to Power BI Service**

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop**
- **DAX** (Data Analysis Expressions) for calculated measures
- **Power Query** for data transformation
- **Treemap, Donut, Line, Combo Bar** native Power BI visuals
- **Chiclet Slicer** custom visual from AppSource

---

## 📋 DAX Measures Used

```dax
Total Billing Amount = SUM(Healthcare[BillingAmount])

Avg Billing Amount = AVERAGE(Healthcare[BillingAmount])

Total Patients = COUNTROWS(Healthcare)

Total Female Patients = 
    CALCULATE(COUNTROWS(Healthcare), Healthcare[Gender] = "Female")

Total Male Patients = 
    CALCULATE(COUNTROWS(Healthcare), Healthcare[Gender] = "Male")
```

---

## 👤 Author

**[MANIKYA]**
- LinkedIn: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/manikya-pasi/)
- GitHub: [github.com/yourusername](https://github.com/Manikya1203)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> ⭐ If you found this project useful, please give it a star!
