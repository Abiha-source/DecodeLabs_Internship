# 📦 Task 1 — Data Collection & Dataset Understanding

**DecodeLabs Data Analytics Internship | Batch 2026**  
**Intern:** Umm-e-Abiha

---

## 🎯 Objective

Load the E-Commerce Orders dataset and develop a comprehensive understanding of its structure, features, data types, and content before any analytical work begins.

---

## 📋 What Was Done

| Step | Action |
|------|--------|
| 1.1 | Loaded `Dataset_for_Data_Analytics.xlsx` using `pandas.read_excel()` |
| 1.2 | Inspected all column names, data types, and sample values |
| 1.3 | Previewed the first 5 rows |
| 1.4 | Generated descriptive statistics for numeric columns |
| 1.5 | Analysed value distributions in categorical columns |
| 1.6 | Produced visualisations (product bar chart + order status pie chart) |

---

## 📊 Dataset Profile

| Attribute | Value |
|-----------|-------|
| Rows | 1,200 |
| Columns | 14 |
| Time Span | January 2023 – June 2025 |
| Memory | ~250 KB |
| Domain | B2C E-Commerce |

---

## 📁 Column Descriptions

| Column | Type | Description |
|--------|------|-------------|
| `OrderID` | Object | Unique order identifier |
| `Date` | Object | Order date (needs parsing in Task 2) |
| `CustomerID` | Object | Unique customer identifier |
| `Product` | Object | Product type (7 categories) |
| `Quantity` | Int | Units per transaction (1–5) |
| `UnitPrice` | Float | Price per unit (USD) |
| `TotalPrice` | Float | Quantity × UnitPrice |
| `OrderStatus` | Object | Fulfilment stage (5 categories) |
| `PaymentMethod` | Object | Payment channel |
| `CouponCode` | Object | Discount code — contains missing values |
| `ReferralSource` | Object | Acquisition channel |
| `ItemsInCart` | Int | Cart size at checkout |

---

## 💡 Key Findings

- **7 product types** are present in equal proportions
- **5 order statuses** are distributed relatively evenly
- **Average order value** is approximately $1,054
- `CouponCode` has **309 missing values** requiring treatment in Task 2
- `Date` is stored as a string (object) and must be converted for time-series analysis

---

## 📁 Output

| File | Description |
|------|-------------|
| `Task_01_Data_Collection.ipynb` | Notebook for this task |
| `task1_overview.png` | Product distribution and order status chart |

---

## 🛠️ Libraries Used

`pandas` · `matplotlib`

---

*DecodeLabs Industrial Training Program | Batch 2026*
