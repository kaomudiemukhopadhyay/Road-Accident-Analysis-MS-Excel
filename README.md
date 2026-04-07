# 🚦 Road Accident Analysis – MS Excel (End-to-End Project)
Developed a Road Accident Analysis project in Excel by performing data cleaning, transformation, and analysis. Used formulas, pivot tables, and charts to calculate KPIs like total casualties, severity distribution, and trends, and created a dashboard for clear insights and reporting.
https://drive.google.com/file/d/1caL5IkQonhKyjK5KXtRcVgBs4kYKLF6b/view?usp=drive_link

Dashboard: <img width="1231" height="590" alt="image" src="https://github.com/user-attachments/assets/22e4fad3-e85e-42d9-b6f0-e31958de3c69" />

Data Analysis :<img width="1185" height="587" alt="image" src="https://github.com/user-attachments/assets/af770f2f-2a44-4d29-a4d3-c2f6cbdde0bb" />


NOTE:📥 Full Dataset (ZIP):
https://your-google-drive-link
Note: Google Drive may show a warning for large files. This is normal and safe to proceed with download.

## 📌 Project Summary

This project presents an end-to-end analysis of road accident data using Microsoft Excel. It includes data cleaning, transformation using Excel formulas, analysis using pivot tables, and dashboard creation to generate meaningful insights and support data-driven decision-making.

---

## 📥 Full Dataset (ZIP)

https://drive.google.com/file/d/1caL5IkQonhKyjK5KXtRcVgBs4kYKLF6b/view?usp=drive_link
> ⚠️ Note: Google Drive may show a warning for large files. This is normal and safe.

---

## 🎯 Business Objective

The objective of this project is to design an interactive dashboard to analyze road accident data for 2021 and 2022 and provide insights into accident patterns, severity, and contributing factors.

---

## 👥 Stakeholders

* Ministry of Transport
* Road Transport Department
* Police & Traffic Authorities
* Emergency Services
* Traffic Management Agencies
* Public & Media

---

# 🧹 1. Data Cleaning

The dataset was prepared using the following steps:

* Removed duplicate records
* Handled missing/null values
* Corrected inconsistent values (Fetal → Fatal)
* Standardized date format
* Ensured correct data types (Date, Number, Text)

👉 Clean data ensures accurate analysis and reliable results.

---

# ⚙️ 2. Data Transformation (Excel Formulas + Logic)

---

## 📅 2.1 Extract Month Name

```excel
=TEXT(B2,"mmm")
```

👉 Converts date into readable month name (Jan, Feb)
👉 Used for dashboard display

---

## 📅 2.2 Extract Year

```excel
=TEXT(B2,"yyyy")
```

👉 Extracts year for yearly comparison

---

## 📅 2.3 Extract Month Number (Sorting Logic 🔥)

```excel
=MONTH(B2)
```

👉 Returns numeric month (1–12)
👉 Used to sort months correctly in pivot tables

---

## 📅 2.4 Extract Year (Numeric)

```excel
=YEAR(B2)
```

👉 Used for filtering and pivot grouping

---

## ⚠️ 2.5 Error Handling

```excel
=IFERROR(A2,0)
```

👉 Replaces errors like #REF!, #DIV/0 with 0

---

## ➕ 2.6 Aggregation Logic

```excel
=SUM(range)
=COUNT(range)
```

👉 Used to calculate totals and counts

---

# 📊 3. Data Analysis (Pivot Tables)

---

## 🔹 3.1 Total Casualties

* SUM(Number_of_Casualties)
* Result: **417,883**

---

## 🔹 3.2 Casualties by Severity

* Fatal → 7,135
* Serious → 59,312
* Slight → 351,436

👉 Slight category contributes the highest casualties

---

## 🔹 3.3 Vehicle Type Analysis

* Cars contribute the highest casualties

👉 Helps identify high-risk vehicle category

---

## 🔹 3.4 Monthly Trend (CY vs PY)

* Rows → Month
* Columns → Year
* Values → SUM(Casualties)

👉 Used for year-over-year comparison

---

## 🔹 3.5 Road Type Analysis

* Single carriageway → highest accidents

---

## 🔹 3.6 Road Surface Analysis

* Dry roads → highest casualties

---

## 🔹 3.7 Urban vs Rural Analysis

* Urban areas → more accidents

---

## 🔹 3.8 Day vs Night Analysis

* Daytime → higher accident rate

---

# 📈 4. Dashboard Development

---

## Components Used:

* KPI Cards → Total casualties
* Line Chart → Monthly trends
* Bar Chart → Road type analysis
* Donut Charts → Area & Time comparison
* Tree Map → Road surface analysis
* Slicers → Interactive filtering (Year, Area)

---

# 🧠 5. Approach (Step-by-Step Thinking)

1. Clean the raw data
2. Transform data using formulas
3. Analyze using pivot tables
4. Identify patterns and insights
5. Build dashboard for visualization

---

# 🔍 6. Key Insights

* Cars contribute the highest casualties
* Urban areas have more accidents
* Daytime accidents are higher
* Dry road conditions have the most accidents
* Single carriageway roads are most risky

---

# 📊 7. Business Impact

This analysis helps stakeholders identify high-risk areas and factors contributing to accidents. It supports better decision-making for road safety improvements, traffic control, and awareness programs.

---

# ⚠️ 8. Challenges & Solutions

| Issue              | Cause              | Solution                 |
| ------------------ | ------------------ | ------------------------ |
| #REF! error        | Broken reference   | Fixed data source        |
| Circular reference | Incorrect formula  | Removed calculated field |
| Wrong month order  | Text sorting issue | Used MONTH()             |
| Pivot not updating | Data changes       | Refreshed pivot          |

---

# 📌 9. Data Assumptions & Validation

* Assumed dataset is complete and accurate
* Handled missing values
* Standardized inconsistent entries
* Verified data types before analysis

---

# 🧰 10. Excel Functions Used

```excel
TEXT(), MONTH(), YEAR(), SUM(), COUNT(), IFERROR()
```

---

# 🎤 11. Interview Explanation

In this project, I cleaned and structured raw accident data, used Excel formulas for transformation, and applied pivot tables to analyze key metrics such as casualties, severity, and trends. Finally, I built an interactive dashboard to present insights effectively.

---

# 🚀 12. Conclusion

This project demonstrates how Excel can be used to transform raw data into meaningful insights using data cleaning, transformation, pivot tables, and dashboard visualization, enabling data-driven decision-making.

---
