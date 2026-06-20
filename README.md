# 🏦 Bank Loan Analysis Project

## 📊 Project Overview
This repository features an end-to-end data analytics project designed to evaluate, track, and optimize a commercial bank's lending operations. Utilizing **SQL** for robust data extraction and auditing, alongside **Power BI** for advanced data modeling and storytelling, this project provides a comprehensive look into portfolio health indicators ($KPIs$), lending trends, risk vectors, and structural compliance margins.

---

## 🖥️ Interactive Dashboards

### 1. Executive Summary Dashboard
*Monitors high-level lending parameters, month-over-month performance shifts, and partitions portfolio health dynamically into Good vs. Bad loan categories.*

![Executive Summary Dashboard](summary_dashboard.png)

### 2. Operational Overview Dashboard
*Provides a multi-dimensional look into geographic disbursement densities, lending purposes, employment durations, and homeownership trends.*

![Operational Overview Dashboard](overview_dashboard.png)

### 3. Granular Details Grid
*An audit-ready, consolidated tabular interface offering full data visibility into borrower metrics for compliance verification.*

![Granular Details Grid](details_dashboard.png)

---

## 🔑 Key Insights & Analytics Features

* **Portfolio Health Tracking:** Monitors critical $KPIs$ including **Total Loan Applications (38.6K)**, **Total Funded Amount (\$435.8M)**, and **Total Amount Received (\$473.1M)**.
* **Risk Categorization (Good vs. Bad Loans):** Segments records to reveal an **86.1% Good Loan** success rate against a **13.9% Bad Loan** default rate to protect bank capital margins.
* **Advanced Time-Intelligence:** Implemented precise dynamic and fixed Month-to-Date ($MTD$), Previous Month-to-Date ($PMTD$), and Month-over-Month ($MoM\%$) calculation logic.
* **Geographic Intelligence:** Features an interactive **Shape Map** tracking state-by-state financial saturation and application density across the United States.

---

## 🛠️ Technical Stack & Implementation

### 1. Data Manipulation & Aggregation (SQL)
* Standardized raw bank records and structured benchmarking metrics.
* Developed validation queries to ensure Power BI calculations tie back identically to source data aggregates.

### 2. Data Modeling & Advanced DAX (Power BI)
* Created a resilient, dynamic string-to-date conversion column (`Issue Date Proper`) to successfully bypass multi-format data-type inconsistencies (`DD-MM-YYYY` vs `M/D/YYYY`).
* Built a custom, fully connected calendar table (`Date-table`) to manage time intelligence cleanly independent of local machine regional configurations.
* Overrode standard `TOTALMTD` limitations on flat data configurations using custom `CALCULATE` filters for flawless row-level cross-filtering inside matrix blocks.

---

## 📂 Repository Structure
* `/Dataset` : Contains the raw financial loan CSV data used for testing and verification.
* `/PowerBI_Report` : Contains the native `.pbix` dashboard file.

---
### 👤 Author
Developed by **Cynthia Ogbekhiulu** * GitHub: [@CynthiaOgbe2907](https://github.com/CynthiaOgbe2907)
