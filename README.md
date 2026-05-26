# 🛒 Integrated Retail Analytics
### Store Optimization & Demand Forecasting

> End-to-end retail analytics pipeline — anomaly detection, customer segmentation, market basket analysis, and demand forecasting on 45-store Walmart sales data.

---

## 📌 Overview

Analyzes **421,570+ weekly sales records** across 45 stores and 81 departments (Feb 2010 – Nov 2012) to extract actionable insights for store optimization, demand planning, and personalized marketing.

---

## 📂 Dataset

| File | Records | Description |
|------|---------|-------------|
| `sales data-set.csv` | 421,570 | Weekly sales per Store × Department |
| `Features data set.csv` | 8,190 | CPI, Fuel Price, Temperature, Unemployment, MarkDowns |
| `stores data-set.csv` | 45 | Store Type (A/B/C) and Size |

---

## 🔬 Project Components

| # | Component | Methods Used |
|---|-----------|-------------|
| 1 | **Exploratory Data Analysis** | Time-series plots, correlation heatmap, groupby aggregation |
| 2 | **Data Preprocessing** | Median imputation, MinMax scaling, sqrt transformation |
| 3 | **Anomaly Detection** | 3-Sigma rule, Isolation Forest, IQR fences |
| 4 | **Time-Based Anomaly Detection** | Rolling avg (26-week window), EWMA (α=0.3) |
| 5 | **Customer Segmentation** | PCA (3 components) + K-Means (k=4), Silhouette analysis |
| 6 | **Market Basket Analysis** | Apriori (support=1.1%, confidence=80%, lift≥3) |
| 7 | **Demand Forecasting** | SARIMAX, Random Forest Regressor, Holt-Winters |
| 8 | **External Factor Analysis** | RF feature importance, pct_change engineering |

---

## 📊 Key Findings

- 🚨 **~1.8% anomaly rate** — 90%+ of anomalies fall on holiday weeks
- 🏪 **4 store clusters** identified: Premium Space, Value-Oriented, Budget-Friendly, Compact Elegance
- 🛍️ **High-confidence association rules** (lift > 3) discovered between department pairs
- 📈 **Random Forest outperforms SARIMAX** on multi-feature test data
- 📅 **2013 full-year forecast** generated via Holt-Winters with validated MAPE

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?logo=scikit-learn)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Time%20Series-4B8BBE)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-76B7B2)

```
pandas · numpy · matplotlib · seaborn
scikit-learn · statsmodels · scipy · apyori
```

---


## 👤 Author

**Shourya Kumar**

---

## 📄 License

This project is for academic purposes only.
