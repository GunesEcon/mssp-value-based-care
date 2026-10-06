# Medicare Shared Savings Program (MSSP) Value-Based Care Analytics

An end-to-end data engineering and analytics pipeline for multi-year Medicare Shared Savings Program (MSSP) public-use data, harmonizing longitudinal performance records, financial results, SNF alignments, Advance Investment Payments (AIP), beneficiary assignment mixes, and county-level expenditure and risk profiles across 2013–2026.

---

## 📁 Core Master Datasets (Project Root)

1. **`mssp_financial_longitudinal_master.csv`** (2013–2024 Financial & Quality Results)
2. **`mssp_county_expenditure_risk_longitudinal_master.csv`** (County-level FFS expenditures & risk scores)
3. **`mssp_aco_organizational_master.csv`** (ACO metadata, SNF affiliates, and AIP spend plans)
4. **`mssp_beneficiary_complexity_master.csv`** (Beneficiary assignment & demographic complexity metrics)

---

## 🚀 Quick Start (Python)

```python
import pandas as pd

# Load the financial longitudinal performance master
df_fin = pd.read_csv("mssp_financial_longitudinal_master.csv", low_memory=False)
print("Financial Master Shape:", df_fin.shape)
