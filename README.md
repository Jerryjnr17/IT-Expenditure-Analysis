# 🧾 IT Expenditure Analysis Dashboard

## 📘 Project Overview
This project focuses on analyzing and visualizing **IT expenditure data** to uncover budget management issues and support better financial control.  
The organization is facing challenges in managing its IT costs, as evident from large variances between **actual**, **planned**, and **forecasted** spending.

The goal of this project is to:
- Identify where these discrepancies occur (by month, business area, country, cost element, and IT area).  
- Understand the root causes behind these variances.  
- Enable better forecasting and financial performance management.

---

## 📊 Dataset Details
**File:** `IT Expenditure dataset.xlsx`

| Column | Description |
|--------|--------------|
| `Date` | Month or period of spending |
| `Business Area` | Department or business unit |
| `Country` | Country of operation |
| `IT Area` | Function or IT domain (e.g., Infrastructure, Applications) |
| `Cost Element Group` | Cost category (Hardware, Software, etc.) |
| `Plan` | Planned IT budget |
| `Forecast` | Forecasted IT expenditure |
| `Actual` | Actual IT expenditure incurred |

---

## 🧹 Data Cleaning Process
Steps performed before analysis:
1. Removed rows where **Actual**, **Plan**, and **Forecast** were all blank.  
2. Standardized column names and data formats.  
3. Converted all financial fields to numeric type.  
4. Extracted **Month** from date field for time-based analysis.  
5. Created new calculated columns:
   - `Variance_vs_Plan = Actual - Plan`  
   - `Variance_%_vs_Plan = (Actual - Plan) / Plan * 100`  
   - `Variance_vs_Forecast = Actual - Forecast`

---

## 🧾 Deliverables
### 1️⃣ Cleaned Data
- Available in `Cleaned_Data` sheet — fully ready for pivot table analysis.

### 2️⃣ Analysis Data
- Includes variance calculations and trend metrics.

### 3️⃣ Dashboard
A colorful and interactive Excel dashboard containing:
- **Summary Cards:** Total Actual, Plan, Forecast, and Variance %  
- **Monthly Trend:** Actual vs Plan line chart  
- **Top Business Areas:** Bar chart of high-variance departments  
- **Top Countries:** Comparison of Actual vs Plan  
- **IT Area Distribution:** Donut chart showing spend share  
- **Cost Element Variance:** Bar chart of major overspending areas  
- **Slicers:** Filters for Country, Business Area, and IT Area  

---

## 🎨 Dashboard Design
A **colorful analytical theme** was used for better clarity and storytelling:
- Palette: Teal, Purple, Coral, Gold  
- Fonts: Calibri / Arial for readability  
- Chart titles, legends, and data labels formatted consistently  
- Clean layout with white background and bright visuals

---

## 🧠 Key Insights (Sample)
- **Variance Trends:** Highest overspend observed in Q3 months.  
- **Business Areas:** Infrastructure and Application Services contributed most to variance.  
- **Countries:** India and the U.S. had the largest deviations vs Plan.  
- **Cost Elements:** Software Licensing and Cloud Services showed consistent overspending.  

---

## ⚙️ How to Use
1. Open `IT_Expenditure_Dashboard.xlsx`.  
2. Go to the **Dashboard** sheet.  
3. Use slicers to filter by Business Area, IT Area, or Country.  
4. Hover or click charts to explore details interactively.  

---

## 🧩 Files Included
| File Name | Description |
|------------|-------------|
| `IT Expenditure dataset.xlsx` | Original dataset |
| `IT_Expenditure_Dashboard.xlsx` | Cleaned and visualized dashboard |
| `README.md` | Project overview and documentation |
| `build_it_dashboard.py` *(optional)* | Python script used for cleaning and automation |

---

## 🧑‍💻 Tools Used
- **Microsoft Excel** – Data cleaning, pivot tables, dashboard creation  
- **Power BI (optional)** – For advanced visualization  
- **Python (pandas, numpy, xlsxwriter)** – For automation and data transformation  

---

## 💡 Recommendations
- Review **monthly variance patterns** to improve future budgeting accuracy.  
- Investigate **IT areas and cost groups** with recurring overspend.  
- Implement real-time tracking dashboards in **Power BI** for continuous monitoring.  

---

## 👨‍💼 Project Context (Crio.Do Data Analyst Project)
This project was developed as part of the **Crio.Do Data Analyst track**.  
It demonstrates skills in:
- Data cleaning and preprocessing  
- Exploratory and variance analysis  
- Excel-based dashboard design and storytelling  
- Communicating insights for business decision-making  

---

**Author:** Vishal  
**Duration:** October 2025  
**Tools:** Excel, Python, Power BI  
**Theme:** Data Analytics for IT Financial Performance
