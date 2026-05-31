# latam-fx-risk-monitor.
Quantitative FX risk monitoring tool for Latin American exporters, Python data pipeline, VaR calculations (COP, MXN, BRL, CLP, ARS), and interactive Power BI dashboard.
# LatAm FX Risk Monitor

> Quantitative exchange rate risk monitoring tool for Latin American exporters.  
> Analyzing COP, MXN, BRL, CLP, and ARS volatility to quantify export revenue exposure.

---

## Overview

Latin American exporters face significant FX risk exposure that is rarely measured with rigorous quantitative tools. This project builds an automated pipeline to monitor historical volatility and calculate Value at Risk (VaR) for 5 LatAm currency pairs against USD, CAD, and EUR — translating statistical risk into actionable dollar-amount exposure for export scenarios.

**Research question:** For a Colombian exporter with $1M USD in annual sales, what is the expected maximum loss from COP/USD volatility at a 95% confidence level over 30, 60, and 90-day windows?

---

## Methodology

- **Data source:** [Frankfurter API](https://www.frankfurter.app/) — free, no API key required
- **Coverage:** 3 years of daily FX data (2022–2025) for COP, MXN, BRL, CLP, ARS
- **Risk metric:** Historical Value at Risk (VaR) at 95% and 99% confidence intervals
- **Visualization:** Interactive Power BI dashboard (3 modules)

---

## Project structure

```
latam-fx-risk-monitor/
│
├── data/               # Raw and cleaned FX datasets
├── notebooks/          # Jupyter notebooks — analysis step by step
│   ├── 01_data_download.ipynb
│   ├── 02_returns_and_volatility.ipynb
│   └── 03_var_calculation.ipynb
├── dashboard/          # Power BI file (.pbix) + screenshots
└── report/             # Methodology paper (English, PDF)
```

---

## Dashboard modules

| Module | Description |
|---|---|
| Historical trends | Daily exchange rate evolution per currency pair with date filters |
| VaR comparison | Cross-country risk comparison at 95% and 99% confidence |
| Scenario simulator | Dynamic export-amount input → expected loss calculation |

---

## Status

- [x] Repository created
- [ ] Data pipeline (Python + Frankfurter API)
- [ ] VaR calculations
- [ ] Power BI dashboard
- [ ] Methodology paper

---

## Author

**Manuela Falla Alcalá** — Undergraduate Researcher, Universidad EAN  
