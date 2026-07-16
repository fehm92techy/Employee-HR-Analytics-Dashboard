# 📊 Enterprise-Grade Employee HR Analytics Application

An interactive, corporate-grade Business Intelligence (BI) application developed to track, model, and diagnose workforce demographics, compensation structures, compliance frameworks, and organizational retention metrics for a scaling enterprise of **5,000 active employees**.

This repository serves as a complete strategic data engineering and analytics case study, demonstrating how raw enterprise resource planning (ERP) transactional systems can be engineered into an interactive reporting application to empower HR Business Partners (HRBPs) and C-suite executives with real-time, data-backed talent strategy.

---

## 🧭 Project Objectives & Core Analytics

In modern corporate environments, managing talent pipelines, auditing payroll leakages, and driving Diversity, Equity, & Inclusion (DE&I) metrics manually is highly inefficient. This project addresses these critical corporate challenges by:
1. **Consolidating Siloed Workforce Data:** Centralizing employee records into a unified, low-latency analytics data model.
2. **Optimizing Compensation Overhead:** Providing granular visual cross-sections of basic salaries vs. gross budgets across different departments.
3. **Mitigating Retention Risks:** Engineering experience-binned workforce tracking to isolate operational bottlenecks and support corporate succession planning.

---

## 📌 Executive Dashboard Architecture & Module Breakdown

The application is architected across **3 highly interactive visual modules**, optimized for rapid executive scanning and strategic drill-downs:

### 🏢 Module 1: Workforce Overview Dashboard (Operational Infrastructure View)
Designed as the primary operational command center to provide global visibility into headcount distribution, regional density, and organizational demographic equilibrium.
* **Core Macro KPI Blocks:** Dynamically aggregates macro-level metrics, showing a total workforce sizing of **5,000 active employees**, an organizational **Average Age of 40 years**, a deeply seasoned **Average Experience of 19 Years**, and an **Average Base Salary of ₹93.86K**.
* **Geographical Spread Matrix:** Features an indexed cross-tabulation table mapping talent distribution across key economic centers, highlighting primary operational hubs in **Delhi (1,322 employees)** and **Mumbai (847 employees)**, followed by regional offices in **Ranchi (208)**, **Hyderabad (175)**, and **Bangalore (172)**.
* **Functional Capacity Sizer:** Uses a horizontal layout to rank organizational team sizes, identifying **Human Resources as the largest function at 1,035 personnel**, followed by **IT (1,005)**, **Sales (1,004)**, **Finance (989)**, and **Marketing (967)**.
* **DE&I Equality Model (Gender Donut):** Mathematically tracks gender diversity splits across the company to verify recruitment equity: **Female (1.67K / 33.48%)**, **Male (1.66K / 33.16%)**, and **Other (1.67K / 33.36%)**.
* **Corporate Insurance Mix Matrix:** Evaluates employee benefit plan enrollments broken down by marital status across four primary wellness categories: **Both benefits (1,292)**, **Life insurance only (1,245)**, **Not Applicable/Opted Out (1,238)**, and **Medical coverage only (1,225)**.

### 💰 Module 2: Financials & Compensation Analysis (Cost Center Control)
A strict financial diagnostic interface optimized for financial controllers and auditors to monitor payroll overheads, tax/fund allocations, and salary progression scaling.
* **Fiscal Footprint KPIs:** Aggregates macro payroll liabilities showing a **Total Gross Budget of ₹550.43M**, a statutory **Total Provident Fund (PF) Contribution of ₹69.61M**, and an **Average Gross Salary of ₹110.09K** per individual.
* **Dual-Axis Payroll Cost Comparison:** Evaluates fiscal variances by contrasting *Sum of Gross Salary* against baseline *Sum of Salary* across business units. The model exposes **Sales at ₹114M** and **Human Resources at ₹112M** as the primary drivers of gross corporate spending.
* **Insurance Cohort Allocation:** Visualizes risk containment patterns via an exact programmatic slice: **Life policies (24.9%)**, **Medical coverage (24.5%)**, **Dual coverage (25.84%)**, and **N/A status (24.76%)**.
* **Tenure Compensation Scale:** Features an analytical line chart mapping salary evolution over a 40-year industry tenure path. It isolates clear corporate promotion steps—such as baseline jumps around year 13 reaching ₹109K, scaling past ₹111K, and peaking at **₹151K** for seasoned 28+ year experts.

### ⏳ Module 3: Talent Pool & Employee Retention (Succession Planning)
A workforce stability module built to track institutional memory, monitor title density, and implement early-warning systems for talent attrition.
* **Workforce Stability KPIs:** Tracks employee attachment and stability indexes, highlighting an elite organizational loyalty score with an **Average Tenure in Company of 9.79 Years** paired with a deep **Average Total Industry Experience of 19.38 Years**.
* **Experience Binning Histograms:** Groups employees into structured experience ranges to monitor workforce maturity. The distribution shows distinct pipeline pillars peaking evenly at the **30-year experience bin (667 employees)** and the newer **5-year group (665 employees)**, balancing historical insight with fresh energy.
* **Designation Headcount Rankings:** Automatically identifies the density of functional roles across the organizational hierarchy, reporting a heavy footprint in technical roles led by **QA Leads (198 personnel)** and **Software Engineers (197)**, closely supported by regional management nodes like **National Sales Managers (196)**, **Senior Executives (195)**, and **Senior HR Professionals (195)**.
* **Granular Audit Ledger:** Integrates a micro-level reference grid displaying specific employee rows (*Name, Department, Position, Years of Experience, In-Company Years*) for direct corporate audits.

---

## 📊 Data Dictionary & Schema Architecture

The underling data structure processes **18 core columns** per employee record. Key engineered attributes include:

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `Name` | Text | Unique identifier for employee profiling. |
| `Department` | Text | Functional cost center assignment (HR, IT, Sales, Finance, Marketing). |
| `Position` | Text | Hierarchical corporate designation (e.g., QA Lead, Software Engineer). |
| `City` | Text | Regional talent hub allocation (Delhi, Mumbai, Bangalore, etc.). |
| `Salary` | Currency (Decimal) | Base monthly/annualized salary footprint. |
| `Gross Salary` | Currency (Decimal) | Total compensation package including calculated allowances. |
| `PF Contribution` | Currency (Decimal) | Statutory provident fund deductions. |
| `Year of Experience` | Integer | Cumulative professional background across the industry. |
| `In Company Years`| Integer | Direct institutional tenure within the current firm. |
| `Insurance` | Text | Core health benefit selections (Both, Medical, Life, N/A). |

---

## 🛠️ Data Engineering & UI Methodology

* **Data Modeling Paradigm:** Implemented an optimized reporting structure within Power BI Desktop, connecting localized lookup dimensions directly to core employee metrics.
* **Advanced UI/UX Canvas:** Styled with a custom, low-latency background canvas (`Power BI Project Lt Background.jpg`) to ensure executive-grade readability, utilizing structured card containers, color-coded donut segments, and synchronized slicers.
* **Dynamic Cross-Filtering:** Equipped with global cross-page slicers (Department, Gender, City, Marital Status, Insurance, and Position) enabling instant ad-hoc drill-downs for executive queries.

---

## 📁 Repository Structure & Artifacts

* 📊 `%EMPL DASHBOARD PBi Project P2 by Fehm .pbix` – The foundational Power BI binary containing compiled data models, entity relationships, custom visual layers, and interactive page layouts.
* 📄 `Power BI Prj 5k dataset Complete_Employee_Dashboard.xlsx` – The master dataset containing 5,000 fully populated employee rows mapped against critical organizational attributes.
* 🎨 `Power BI Project Lt Background.jpg` – The tailored visual background layer designed to provide clean, clutter-free structural frames for all charts.
