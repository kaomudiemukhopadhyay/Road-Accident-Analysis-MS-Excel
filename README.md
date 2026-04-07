# Road-Accident-Analysis-MS-Excel
Developed a Road Accident Analysis project in Excel by performing data cleaning, transformation, and analysis. Used formulas, pivot tables, and charts to calculate KPIs like total casualties, severity distribution, and trends, and created a dashboard for clear insights and reporting.
https://drive.google.com/file/d/1caL5IkQonhKyjK5KXtRcVgBs4kYKLF6b/view?usp=drive_link


NOTE:📥 Full Dataset (ZIP):
https://your-google-drive-link
Note: Google Drive may show a warning for large files. This is normal and safe to proceed with download.


# 📄 Road Accident Analysis – Excel Project
## 📌 1. Project Overview
This project focuses on analyzing road accident data using Excel. The aim is to clean raw data, process it into a structured format, perform analysis using pivot tables, and build an interactive dashboard to generate insights.


## 📌 2. Business Requirement
The goal is to create a Road Accident Dashboard for the years 2021 and 2022.
The dashboard should provide:
* Total casualties
* Severity-wise breakdown (Fatal, Serious, Slight)
* Vehicle type analysis
* Monthly trend comparison (CY vs PY)
* Road type and road surface insights
* Urban vs Rural distribution
* Day vs Night analysis

## 👥 3. Stakeholders

* Ministry of Transport → Policy decisions
* Road Transport Department → Road improvement
* Police → Law enforcement
* Emergency Services → Quick response
* Traffic Agencies → Traffic management
* Public → Awareness
* Media → Reporting

---

## 🧹 4. Data Cleaning (Step-by-Step)

Raw data is messy, so cleaning is required.

### Actions Performed:

* Removed duplicates → Data → Remove Duplicates
* Handled blank/null values
* Corrected spelling (Fetal → Fatal)
* Standardized date format
* Ensured correct data types

---

## ⚙️ 5. Data Processing (IMPORTANT)

Created new columns for analysis.

### 📅 Extract Month Name

```excel
=TEXT(B2,"mmm")
```

### 📅 Extract Year

```excel
=TEXT(B2,"yyyy")
```

### 📅 Extract Month Number (for sorting)

```excel
=MONTH(B2)
```

### 📅 Extract Year (numeric)

```excel
=YEAR(B2)
```

👉 These columns are used in pivot tables.

---

## 📊 6. Data Analysis (Pivot Tables)

---

### 🔹 6.1 Primary KPI – Total Casualties

👉 Pivot:

* Values → SUM(Number_of_Casualties)

👉 Output:
Total = **417,883**

---

### 🔹 6.2 Casualties by Severity

👉 Rows:

* Accident Severity (Fatal, Serious, Slight)

👉 Values:

* SUM(Number_of_Casualties)

👉 Output:

* Fatal → 7,135
* Serious → 59,312
* Slight → 351,436



### 🔹 6.3 Casualties by Vehicle Type

👉 Grouped into:

* Cars
* Van
* Bus
* Bike
* Agricultural
* Others

👉 Output example:

* Cars → 333,485 (Highest)



### 🔹 6.4 Monthly Trend (2021 vs 2022)

👉 Rows:

* Month

👉 Columns:

* Year

👉 Values:

* SUM(Number_of_Casualties)

👉 Insight:
Compare trends between years.

---

### 🔹 6.5 Casualties by Road Type

👉 Rows:

* Road Type

👉 Values:

* SUM(Number_of_Casualties)

👉 Example:

* Single carriageway → Highest

---

### 🔹 6.6 Casualties by Road Surface

👉 Rows:

* Road Surface

👉 Values:

* SUM(Number_of_Casualties)

👉 Example:

* Dry → Highest

---

### 🔹 6.7 Urban vs Rural

👉 Rows:

* Urban / Rural

👉 Values:

* SUM(Number_of_Casualties)

---

### 🔹 6.8 Day vs Night

👉 Rows:

* Light Condition

👉 Values:

* SUM(Number_of_Casualties)

---

## 📈 7. Dashboard Creation

---

### Components Used:

* KPI Cards (Top section)
* Line Chart → Monthly trend
* Bar Chart → Road type
* Donut Chart → Urban vs Rural
* Donut Chart → Day vs Night
* Tree Map → Road surface
* Slicers → Year, Area

---

## 🎨 8. Dashboard Design

* Dark theme background
* Highlight KPIs in top section
* Consistent colors for charts
* Icons used for better UI

---

## 🧠 9. Step-by-Step Thinking

1. Data is messy → Clean
2. Data is ready → Process
3. Data is structured → Analyze
4. Data insights → Dashboard

---

## 🎤 10. Interview Explanation

In this project, I cleaned the dataset by handling missing values and correcting inconsistencies. Then I created new columns like month and year using Excel formulas. I used pivot tables to analyze the data and calculate KPIs such as total casualties, severity distribution, and trends. Finally, I built an interactive dashboard to visualize insights.

---

## 🎯 11. Key Insights

* Cars contribute highest casualties
* Urban areas have more accidents
* Daytime accidents are higher
* Dry roads have most accidents
* Single carriageway is most risky

---

## ⚠️ 12. Errors Faced & Solution

### Issue:

* #REF! error in pivot
* Circular reference

### Solution:

* Removed calculated field
* Checked data source
* Refreshed pivot
* Recreated pivot

---

## 📌 13. Important Excel Functions Used

```excel
=TEXT(B2,"mmm")
=TEXT(B2,"yyyy")
=MONTH(B2)
=YEAR(B2)
=SUM(range)
=COUNT(range)
=IFERROR(value,0)
```

---

## 🚀 14. Conclusion

This project demonstrates how Excel can be used for complete data analysis, from cleaning raw data to building a professional dashboard. It helps in understanding accident trends and supports data-driven decision-making.

---
