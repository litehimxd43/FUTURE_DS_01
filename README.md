# Online Retail Analytics & Executive Dashboard

An end-to-end exploratory data analysis (EDA) and executive business intelligence pipeline built with Python. This project ingests transactional e-commerce data, performs schema validation and data hygiene, calculates core business metrics, and automatically compiles multi-panel executive dashboards into a presentation-ready PDF report.

---

## Features

- **Automated Data Hygiene & Cleaning**: Filters cancelled orders (`InvoiceNo` prefix `C`), negative or zero quantities, and invalid unit prices.
- **Feature Engineering**: Derives temporal dimensions (`YearMonth`, `Hour`, `DayOfWeek`) and computes gross transaction values (`TotalPrice`).
- **Commercial Performance Tracking**:
  - Key Performance Indicators (Total Revenue, Transaction Volume, Unique Customers, Average Order Value).
  - Monthly revenue trajectories and seasonal demand forecasting (e.g., Q4 holiday surges).
  - Intraday buying velocity and day-of-week sales concentration.
- **Market & Product Diagnostics**:
  - Domestic vs. international export market distribution.
  - Price elasticity modeling (Unit Price vs. Quantity on a log-log scale).
  - SKU Pareto analysis (top revenue-generating products).
  - Customer lifetime value (CLV) distribution and top VIP account ranking.
- **Direct PDF Export**: Uses `matplotlib.backends.backend_pdf.PdfPages` to compile multi-panel visual boards directly into a high-resolution (300 DPI) PDF document.

---
