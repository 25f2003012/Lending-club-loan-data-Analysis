# 📊 Lending Club Loan Risk & Portfolio Analytics

![Power BI]
![Python]
![Pandas]
![Seaborn]

## 📌 Business Problem & Overview
Lending Club is a peer-to-peer lending platform. The primary business challenge in loan underwriting is to balance profitability with credit risk. 

The objective of this project is to perform **Exploratory Data Analysis (EDA)** using Python and build an **Interactive Executive Power BI Dashboard** to identify key risk drivers behind loan defaults (**Charged-Off loans**) and provide actionable insights for credit risk mitigation.

---

## 🎯 Key Metrics & KPIs Tracked
* **Total Portfolio Value ($):** Overall amount lent across all applications.
* **Total Charge-Off Loss ($):** Cumulative financial loss incurred due to defaulted loans.
* **Charge-Off Rate (%):** Primary risk benchmark measuring default frequency.
* **Average DTI Ratio (%):** Measure of borrower debt capacity and leverage risk.
* **Weighted Average Interest Rate (%):** Portfolio risk-yield profile.

---

## 🔍 Key Insights & Findings

1. **Loan Term Impact:** 60-month loans exhibit a significantly higher charge-off rate compared to 36-month loans due to extended financial vulnerability.
2. **Sub-Grade Risk:** Borrowers in lower grades (E, F, G) present the highest probability of default, requiring stricter underwriting controls.
3. **Debt Burden (DTI):** High Debt-to-Income ratios (>20%) strongly correlate with loan defaults, especially when paired with high installment amounts.
4. **Public Rec Bankruptcies:** Prior public bankruptcy records serve as a strong leading indicator for future default.

---

## 🛠️ Project Architecture & Tech Stack

* **Data Processing & EDA (Python):** `Pandas`, `NumPy`
* **Data Visualization (EDA):** `Seaborn`, `Matplotlib` (Bivariate feature analysis using custom distributions)
* **Dashboarding & Business Intelligence:** `Power BI Desktop`
  * **Dynamic Field Parameters:** Single-chart dynamic risk factor analyzer.
  * **DAX & Smart Narrative:** Dynamic textual summaries and custom measures.
  * **Design & Usability:** Clean, high-contrast light theme with floating card visual hierarchy.

---

## 🖥️ Power BI Dashboard Features

* **Interactive Risk Factor Slicer:** Allows users to dynamically select any borrower feature (Grade, Term, DTI, Purpose, Interest Rate) to analyze its relationship with Charge-off rates on a single dynamic chart.
* **Smart Dynamic Insights:** Auto-generating text summary card explaining the top risk segment based on the active selection.
* **Conditional Formatting:** Color-coded KPI alerts highlighting elevated risk thresholds.

---

## 🚀 Strategic Recommendations

* **Cap DTI Limits:** Implement stricter DTI limits specifically for longer-term (60-month) loan applications.
* **Enhanced Verification:** Enforce mandatory income/employment verification for applicants assigned Grade E, F, or G.
* **Early Warning Indicators:** Set up early payment monitoring for high-installment borrowers within the first 6 months of loan origination.

---

## 📂 Repository Structure

```text
├── Data/                       # Raw and processed datasets
├── Notebooks/                  # Python Jupyter Notebook (Bivariate & EDA analysis)
├── Dashboard/                  # Power BI (.pbix) file
├── Assets/                     # Dashboard screenshots / demo GIFs
└── README.md                   # Project documentation
