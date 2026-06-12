# 🚲 Bike Sales Dashboard — Excel Data Analysis Project

An end-to-end data cleaning and interactive dashboard project built in Microsoft Excel, analysing the purchase behaviour of 1,000 customers to understand what factors influence bike buying decisions.

---

## 📌 Project Description

This project takes a raw customer dataset and transforms it into a clean, structured workbook with an interactive visual dashboard. It covers the full data analytics pipeline — from cleaning messy data to building pivot tables, charts, and slicer-driven filters — all within Excel.

The dataset contains demographic and financial information about 1,000 individuals, and the goal is to identify patterns in who buys bikes based on income, gender, age group, and commute distance.

---

## 📂 Repository Structure
Bike-Sales-Ecxel-dashboard/

│

├── Bike_Sales_Dashboard.xlsx   # Main Excel workbook (cleaned data + dashboard)

├── Excel_Project_Dataset.xlsx  # Original raw dataset

└── README.md                   # Project documentation
---

## 🗂️ Dataset Overview

The raw dataset contains **1,026 rows** (including duplicates) and **13 columns**:

| Column | Description |
|---|---|
| ID | Unique customer identifier |
| Marital Status | Married / Single |
| Gender | Male / Female |
| Income | Annual salary |
| Children | Number of children |
| Education | Highest qualification attained |
| Occupation | Type of job |
| Home Owner | Whether the person owns a home |
| Cars | Number of cars owned |
| Commute Distance | Distance between home and workplace |
| Region | Geographic region (Europe, Pacific, North America) |
| Age | Age in years |
| Purchased Bike | Whether the person bought a bike (Yes / No) |

---

## 🧹 Data Cleaning Steps

The following cleaning operations were performed on the raw data:

1. **Removed 26 duplicate rows** — brought the dataset down to 1,000 unique records
2. **Standardised Marital Status** — replaced `M` → `Married` and `S` → `Single`
3. **Standardised Gender** — replaced `M` → `Male` and `F` → `Female`
4. **Formatted Income as Currency** — values displayed in `$` format
5. **Renamed Commute Distance** — `10+ Miles` relabelled as `More than 10 Miles` for clarity
6. **Created Age Group column** — customers classified into three segments:
   - `Adolescent` — under 31 years
   - `Middle Aged` — 31 to 54 years
   - `Old Age` — above 54 years

---

## 📊 Dashboard & Visualisations

The **Dashboard** sheet presents a summary view with:

- **4 KPI Cards** — Total Customers, Bike Buyers, Purchase Rate, Average Income
- **3 Interactive Charts** connected to pivot tables
- **3 Slicers** for dynamic filtering (Marital Status, Region, Education)

### Chart 1 — Average Income by Gender & Bike Purchase
- **Type:** Clustered Bar Chart
- **Insight:** Compares the average income of bike buyers vs non-buyers, split by gender

### Chart 2 — Bike Purchases by Commute Distance
- **Type:** Line Chart
- **Insight:** Shows how commute distance affects the likelihood of purchasing a bike

### Chart 3 — Bike Purchases by Age Group & Gender
- **Type:** Line Chart with Markers
- **Insight:** Breaks down bike buying across Adolescent, Middle Aged, and Old Age groups for both males and females

---


---

## 🛠️ Tools Used

- **Microsoft Excel** — Data cleaning, pivot tables, charts, dashboard
- **Python (openpyxl, pandas)** — Automated data cleaning and workbook generation
- **VBA** — Slicer creation and pivot table connections

---

## 📈 Key Findings

- **Middle Aged customers** (31–54) account for the vast majority of bike purchases across both genders
- Customers with **shorter commutes (0–1 miles)** purchase bikes the most
- **Male buyers** tend to have a slightly higher average income than female buyers
- Purchase rate across the full dataset is approximately **48%**

---


