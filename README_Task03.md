# 📊 Task 3 — Exploratory Data Analysis (EDA)

**DecodeLabs Data Analytics Internship | Batch 2026**  
**Intern:** Umm-e-Abiha

---

## 🎯 Objective

Systematically explore the cleaned dataset to uncover statistical patterns, business metrics, outliers, correlations, and revenue trends that form the foundation of data-driven decision-making.

---

## 📋 What Was Done

| Section | Analysis |
|---------|----------|
| 3.1 | Descriptive statistics (mean, median, std, quartiles) |
| 3.2 | Key business KPIs (AOV, total revenue, coupon rate, top product) |
| 3.3 | Outlier detection using the IQR method |
| 3.4 | Correlation matrix for numeric variables |
| 3.5 | Revenue breakdown by product |
| 3.6 | Revenue breakdown by order status |
| 3.7 | Monthly revenue trend |
| 3.8 | 6-panel EDA visualisation dashboard |

---

## 📈 Key Business KPIs

| Metric | Value |
|--------|-------|
| Average Order Value | ~$1,054 |
| Median Order Value | ~$824 |
| Total Revenue | ~$1,264,800 |
| Highest Single Order | ~$3,456 |
| Coupon Usage Rate | ~26% |
| Top Product (Revenue) | Chair |
| Top Referral Source | Instagram |

---

## 🔍 Outlier Analysis (IQR Method)

| Column | Outliers Found | Interpretation |
|--------|---------------|----------------|
| TotalPrice | 8 | High-value VIP orders — real signal |
| UnitPrice | 0 | Prices are within expected range |
| Quantity | 0 | Order quantities are well-bounded |
| ItemsInCart | 0 | Cart sizes are normal |

---

## 🔗 Correlation Summary

| Variable Pair | Correlation | Strength |
|---------------|-------------|----------|
| UnitPrice ↔ TotalPrice | ~0.72 | Strong positive |
| Quantity ↔ TotalPrice | ~0.62 | Moderate positive |
| Quantity ↔ ItemsInCart | ~0.65 | Moderate positive |

---

## 💡 Key Findings

- **Distribution is right-skewed** (Mean > Median): a small number of high-value orders inflate the average
- **Chair** consistently ranks #1 in total revenue
- **Instagram** is the highest-converting referral channel
- Cancelled orders still carry revenue — indicates high-value customers may be changing their minds

---

## 📁 Output

| File | Description |
|------|-------------|
| `Task_03_EDA.ipynb` | Notebook for this task |
| `task3_eda.png` | 6-panel EDA dashboard |

---

## 🛠️ Libraries Used

`pandas` · `numpy` · `matplotlib`

---

*DecodeLabs Industrial Training Program | Batch 2026*
