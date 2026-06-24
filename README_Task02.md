# 🧹 Task 2 — Data Cleaning & Preprocessing

**DecodeLabs Data Analytics Internship | Batch 2026**  
**Intern:** Umm-e-Abiha

---

## 🎯 Objective

Transform the raw dataset into a clean, validated, and analysis-ready format by systematically resolving all data quality issues and documenting every change.

---

## 📋 What Was Done

| Change ID | Step | Action | Impact |
|-----------|------|--------|--------|
| CR-001 | Missing Value Treatment | Imputed 309 `CouponCode` NaN → `NO_COUPON` | 309 records preserved |
| CR-002 | Duplicate Detection | Scanned for and confirmed 0 duplicate rows | No data lost |
| CR-003 | Date Parsing | Converted `Date` to `datetime`; extracted `Year`, `Month`, `MonthName` | Time-series analysis enabled |
| CR-004 | TotalPrice Validation | Verified `TotalPrice = Quantity × UnitPrice` for all rows | 0 mismatches — data accurate |
| CR-005 | Text Standardisation | Applied `str.strip().str.title()` to all categorical columns | Consistent category labels |

---

## 🔍 Missing Value Audit

| Column | Missing Count | % Missing | Treatment |
|--------|--------------|-----------|-----------|
| `CouponCode` | 309 | 25.75% | Imputed with `NO_COUPON` |
| All others | 0 | 0.00% | No action required |

---

## 💡 Key Decisions

### Why impute instead of delete?
Deleting 309 rows would remove 25.75% of the dataset. A missing `CouponCode` is semantically meaningful — it indicates the customer did not apply a coupon. Imputation preserves all data while maintaining analytical integrity.

### Why validate TotalPrice?
Computational errors in derived columns are common. Verifying `Qty × UnitPrice = TotalPrice` ensures that downstream revenue calculations are based on accurate data.

---

## 📁 Output

| File | Description |
|------|-------------|
| `Task_02_Data_Cleaning.ipynb` | Notebook for this task |
| `task2_cleaning.png` | Before/after missing values + payment method chart |

---

## 🛠️ Libraries Used

`pandas` · `matplotlib`

---

> *"80% of a Data Scientist's work is data preparation; only 20% is analysis."*  
> — Industry Principle

---

*DecodeLabs Industrial Training Program | Batch 2026*
