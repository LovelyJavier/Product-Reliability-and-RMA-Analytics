<div align="center" style="background-color:#F8BBD9; padding:15px; border-radius:8px;">

# <span style="color:#1F3A5F;">Product Reliability and RMA Analytics</span>

</div>

## 1. Project Overview

Analyzed field quality RMA data to assess product reliability, compare manufacturing cohort performance, identify failure trends, and monitor product performance throughout its lifecycle.

**Tools:** Excel, Power Query, Pivot Tables, Excel Formulas

---

## 2. Dashboard Overview

<p align="center">
  <img src="images/dashboard-overview.png" width="100%">
</p>

---

## 3. Business Questions

- What is the overall Return Material Authorization (RMA) rate in the field?
- Which manufacturing cohorts (based on production period) have the highest and lowest RMA rates?
- When do RMAs occur most frequently by month and work week?
- How does the cumulative RMA rate change as each quarterly manufacturing cohort ages?
- Which manufacturing cohorts and time periods exhibit the highest cumulative RMA rates?
- How do cumulative RMA rates vary across aging intervals for each manufacturing cohort?
- Which product categories contribute the most failures?
- What are the most common failure modes reported by customers?

## 4. Data Preparation

| **Step** | **Description** |
|-----------|-----------------|
| **Data Sources** | Combined two Field Quality RMA and manufacturing data sources into a single dataset using **Power Query**. |
| **Data Cleaning** | Used **Power Query** and **Excel formulas** to remove duplicates, correct data types, handle missing values, and clean and standardize text fields. |
| **Text Extraction** | Extracted serial numbers and other relevant information from semi-structured notes using **Power Query** and **Excel formulas**. |
| **Data Standardization** | Developed custom **Spelling Correction** and **Failure Mapping** tables to correct spelling variations, standardize inconsistent issue descriptions, and classify failures into standardized failure modes, categories, and failure types. |
| **Data Integration** | Merged and matched multiple datasets using **Power Query** to create a unified, analysis-ready dataset. |
| **Output** | Produced a clean, consistent, and structured dataset to support RMA trend analysis and interactive dashboard reporting. |

---

## 5. Data Validation

**Objective:** Verify that the total number of RMA records in the dashboard matches the cleaned dataset.

**Validation:** Compared the total RMA count from the cleaned Power Query output with the Pivot Table summary and dashboard KPI.

**Result:** All totals matched, confirming that no records were lost or duplicated during data preparation.

**Steps:**

1. Apply dashboard filters.
2. Verify dashboard result (**38 RMAs**).
3. Apply the same filters to the source dataset.
4. Confirm source record count = **38**.
