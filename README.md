# 🏦 Banking Risk & Loan Analytics Dashboard

An end-to-end banking analytics project that transforms raw client and loan data into actionable risk intelligence — using Power BI to surface credit risk patterns, loan performance trends, and client behavior across a 3,000-record dataset.

### 📌 Project Overview

This project analyzes banking client profiles and loan portfolios to help financial institutions make data-driven decisions around credit risk, loan approvals, and customer segmentation. It delivers a multi-page interactive Power BI dashboard backed by a structured dataset, an Exploratory Data Analysis (EDA) file, and a comprehensive written report.

**Business Goal:** Identify high-risk loan segments, understand client demographics driving default behavior, and provide lending teams with clear visual intelligence to guide underwriting and portfolio management decisions.

---

### 🗂️ Repository Structure

```text
Banking-Risk-Loan-Analytics-Dashboard/
│
├── Banking.csv                        # Primary dataset — loan & client records (3,000 rows)
├── banking-clients.csv                # Client profile dataset (3,000 rows, 567 KB)
├── bankeda.ipynb                      # Exploratory Data Analysis (EDA) notebook
├── Banking Dashboard.pbix             # Power BI dashboard (v1)
├── Banking Dashboard_.pbix            # Power BI dashboard (v2 — refined)
├── Banking Report.docx                # Full written analysis report (1.05 MB)
├── Banking.xlsx                       # Excel version of the dataset
├── Banking.pptx                       # Presentation summarizing key findings
├── Screenshot 2026-05-04 134634.png   # Dashboard page 1 — Overview
├── Screenshot 2026-05-04 134649.png   # Dashboard page 2 — Loan Analysis
├── Screenshot 2026-05-04 134707.png   # Dashboard page 3 — Risk Breakdown
└── Screenshot 2026-05-04 134714.png   # Dashboard page 4 — Client Demographics

```

---

### 🔧 Tools & Technologies

| Tool | Purpose |
| --- | --- |
| **Power BI** | Interactive multi-page dashboard and data modeling |
| **Python / Jupyter** | Exploratory Data Analysis (EDA) via the `bankeda` file |
| **Excel (.xlsx)** | Data preparation and preliminary analysis |
| **Microsoft Word (.docx)** | Written business report with full findings |
| **PowerPoint (.pptx)** | Stakeholder presentation of key insights |
| **CSV datasets** | Raw data source — loan records and client profiles |

---

### 📊 Dataset

**Files:** `Banking.csv` and `banking-clients.csv` | **Size:** 3,000 records each · 567 KB

The datasets contain banking client and loan information covering demographics, financial history, and loan characteristics:

| Field | Description |
| --- | --- |
| **client_id** | Unique identifier for each customer |
| **age / age_group** | Customer age and segmented bracket |
| **gender** | Male / Female |
| **income** | Annual income of the client |
| **employment_status** | Employed / Self-employed / Unemployed |
| **loan_amount** | Value of the loan issued |
| **loan_type** | Personal / Home / Auto / Business / Education |
| **loan_term** | Repayment duration (months) |
| **interest_rate** | Annual interest rate on the loan (%) |
| **loan_status** | Current / Defaulted / Paid Off |
| **credit_score** | Client credit score at time of application |
| **previous_defaults** | Number of prior defaults on record |
| **balance** | Current account balance |
| **region** | Geographic region of the client |

---

### 📈 Dashboard Pages

The Power BI dashboard is structured across 4 analytical pages:

1. **Page 1 — Executive Overview:** High-level KPIs: total loan portfolio value, number of active loans, overall default rate, and average credit score across the client base.
2. **Page 2 — Loan Performance Analysis:** Breakdown of loan status (Current / Defaulted / Paid Off) by loan type, loan amount bands, and repayment term. Trend analysis of loan disbursements over time.
3. **Page 3 — Risk & Default Analysis:** Deep dive into default drivers: credit score distribution among defaulters vs. non-defaulters, correlation between income levels and default rates, and impact of previous defaults on current loan risk.
4. **Page 4 — Client Demographics:** Revenue and loan exposure by age group, gender, employment status, and region — enabling segment-level risk profiling.

---

### 📊 Key Outcomes & Numerical Insights

The following figures are derived from the 3,000-record banking dataset analyzed in this project.

**🏦 Portfolio Overview**

* Total dataset size: 3,000 client loan records covering multiple loan types and risk profiles
* The dataset spans 5 loan categories: Personal, Home, Auto, Business, and Education loans
* Two data perspectives are provided: loan-level transactions (`Banking.csv`) and client-level profiles (`banking-clients.csv`), enabling both portfolio-level and customer-level analysis

**⚠️ Risk & Default Patterns**

* Clients with prior default history are significantly more likely to default again — previous defaults are among the strongest predictors of current loan risk
* Lower credit score bands (typically below 580) are associated with disproportionately higher default rates compared to clients with scores above 700
* Unsecured loan types (Personal, Education) tend to carry higher default risk compared to secured loans (Home, Auto) where collateral reduces lender exposure
* Clients with lower income brackets combined with high loan-to-income ratios represent the highest-risk segment in the portfolio

**👥 Client Demographics & Segmentation**

* Employment status is a strong differentiating factor — unemployed or self-employed clients show higher default concentration than salaried employees
* Age-based segmentation reveals that younger borrowers (18–30) tend to have lower credit scores and shorter credit histories, contributing to elevated risk in that group
* Regional analysis uncovers geographic concentration risk, with certain regions showing above-average default clusters

**💰 Loan Performance Metrics**

* Loan performance varies significantly by loan term length — shorter-term loans generally show better repayment adherence than longer-term ones in the dataset
* Interest rate bands correlate with risk tier: higher-rate loans (typically issued to riskier clients) show correspondingly higher default rates, validating the bank's risk-based pricing model
* The Paid Off segment provides a reference profile of successful borrowers — higher credit scores, stable employment, and lower loan-to-income ratios dominate this group

**📊 Dashboard KPIs**

* The dashboard surfaces 4 core risk dimensions in real time: portfolio health, loan-type performance, client risk segmentation, and demographic exposure
* Cross-filter interactivity allows drilling into any combination of loan type × age group × region × risk status in a single click
* The written report (`Banking Report.docx`) provides a full narrative interpretation of all dashboard metrics with supporting data tables

---

### 🚀 Getting Started

**Prerequisites**

* Power BI Desktop (free download from Microsoft)
* Microsoft Excel (for `.xlsx` data review)
* Any CSV viewer or Python/pandas for raw data exploration

**Steps**

1. **Clone the repository**
```bash

```



git clone https://github.com/sairamanaj/Banking-Risk-Loan-Analytics-Dashboard.git
cd Banking-Risk-Loan-Analytics-Dashboard

```
2. **Review the EDA** Open the `bankeda` file to view the exploratory data analysis and initial data profiling.
3. **Open the dashboard** Launch `Banking Dashboard_.pbix` in Power BI Desktop to interact with the full dashboard. Use built-in slicers to filter by loan type, region, age group, and risk status.
4. **Review the report** Open `Banking Report.docx` for the full written analysis with findings, methodology, and recommendations.
5. **Explore the data** Open `Banking.csv` or `Banking.xlsx` to inspect raw records and understand the underlying data structure.
6. **View the presentation** Open `Banking.pptx` for a slide-based summary of key findings — useful for stakeholder communication.

---

### 💡 Business Recommendations

Based on the analysis:
* **Tighten underwriting for high-risk profiles** — clients with previous defaults + low credit scores + high loan-to-income ratios should face stricter approval criteria or require collateral.
* **Introduce risk-based loan caps** — set loan amount ceilings per risk tier to limit portfolio exposure from the highest-default segments.
* **Target the Paid Off segment for retention** — these customers have demonstrated repayment reliability; proactively offer them renewal or product cross-sell opportunities.
* **Regional risk monitoring** — regions with above-average default clusters warrant closer monitoring and potentially adjusted lending parameters.
* **Employment verification at origination** — employment status is a strong default predictor; robust verification processes at application stage can reduce downstream risk.
* **Credit score improvement programs** — partnering with clients in the 580–650 range with financial literacy or credit-building products could improve portfolio quality over time.

---

### 📁 Deliverables Summary

| Deliverable | Format | Description |
| :--- | :--- | :--- |
| **Interactive Dashboard** | `.pbix` | Multi-page Power BI dashboard with slicers |
| **Exploratory Data Analysis** | `.ipynb` / Python | Comprehensive data profiling (`bankeda`) |
| **Written Report** | `.docx` | Full analytical narrative and findings |
| **Presentation** | `.pptx` | Stakeholder-ready slide deck |
| **Raw Dataset** | `.csv` / `.xlsx` | 3,000-record banking client and loan data |
| **Dashboard Screenshots** | `.png` | 4 static previews of dashboard pages |

---

### 👤 Author
[Sairamana_j GitHub Profile](https://github.com/sairamanaj)

### 📄 License
This project is open-source and available for educational and portfolio use.

```
