# Biomarker-Driven Risk Stratification & Treatment Alignment in Lung Adenocarcinoma (LUAD)

## Project Overview

This project focuses on building a biomarker-driven clinical analytics framework for Lung Adenocarcinoma (LUAD) patients using genomic, transcriptomic, and clinical data. The objective is to identify high-risk and low-risk patient groups based on biomarker expression and mutation patterns, analyze survival outcomes, and create interactive Tableau dashboards for treatment-oriented decision support.

The project combines:

* Clinical data analysis
* Biomarker expression analysis
* Survival-based risk stratification
* SQL-based data integration
* Tableau data visualization
* Exploratory statistical modeling

The final outcome is an interactive analytics solution that helps understand how biomarker profiles influence prognosis and treatment alignment.

### Disclaimer

This project was undertaken as part of the Data Analytics Bootcamp (Dec 2025 – Apr 2026) at Neuefische GmbH, Berlin. The project was completed over four weeks and involved data retrieval, data understanding, integration, analysis, and insight generation using clinical and biomarker datasets.

This project is intended for educational and analytical purposes only. It is not designed for direct clinical diagnosis or medical decision-making.
---

# Problem Statement

Lung Adenocarcinoma is one of the most common and heterogeneous forms of lung cancer. Patients with similar clinical staging often show significantly different treatment responses and survival outcomes due to underlying molecular and genomic differences.

Traditional clinical factors alone are insufficient for accurate prognosis prediction. Therefore, this project explores whether biomarker expression patterns and genomic mutations can be used to:

* Stratify patients into different risk categories
* Identify survival-associated biomarkers
* Analyze treatment relevance using biomarker-driven insights
* Support precision medicine approaches through visual analytics

---

# Objectives

* Integrate clinical and genomic datasets into a unified analytical model
* Analyze biomarker expression patterns in LUAD patients
* Create high-risk and low-risk patient groups using biomarker combinations
* Evaluate survival trends across risk groups, cancer stages, and age groups
* Build interactive Tableau dashboards for exploratory clinical analytics
* Derive actionable insights for treatment alignment and prognosis assessment

---

# Dataset Information

The dataset was created by integrating clinical and expression data using Python and SQL.

## Key Features Used

| Feature                 | Description                      |
| ----------------------- | -------------------------------- |
| patient_id              | Unique patient identifier        |
| sample_id               | Sample identifier                |
| diagnosis_age           | Age at diagnosis                 |
| cancer_stage            | Clinical cancer stage            |
| overall_survival_months | Survival duration in months      |
| overall_survival_status | Survival outcome                 |
| mutation_count          | Total mutation burden            |
| msi_mantis_score        | Microsatellite instability score |
| tmb_nonsynonymous       | Tumor mutation burden            |
| buffa_hypoxia_score     | Hypoxia-related score            |
| EGFR                    | EGFR biomarker expression        |
| KRAS                    | KRAS biomarker expression        |
| ALK                     | ALK biomarker expression         |
| ERBB2                   | ERBB2 biomarker expression       |
| CD274                   | PD-L1 biomarker expression       |

## Data Cleaning

* Removed records with missing survival duration values
* Standardized categorical variables
* Generated binary survival outcome field
* Integrated genomic and clinical information into a single analytical dataset

## Final Dataset

* Initial patient records: 566
* Final cleaned dataset: 505 patients

---

# Methodology

## 1. Data Collection & Integration

Clinical and genomic datasets were processed using Python and integrated into a relational SQL dataset.

### Tools Used

* Python (Pandas, NumPy)
* SQL
* Tableau

---

## 2. Biomarker-Based Risk Stratification

Patients were grouped into risk categories using biomarker expression patterns.

### Example Risk Logic

* High ALK expression + Low KRAS expression → Lower risk group
* Low ALK expression + High KRAS expression → Higher risk group

The project evaluates whether biomarker combinations correlate with:

* Overall survival
* Disease progression trends
* Clinical stage severity
* Age-related prognosis

---

## 3. Survival Analysis

Survival trends were analyzed across:

* Risk groups
* Cancer stages
* Age groups
* Biomarker expression categories

Key metrics analyzed:

* Median survival months
* Event rate
* Survival distribution
* Mortality trends

---

## 4. Exploratory Statistical Analysis

The project includes exploratory statistical modeling and correlation analysis between biomarkers and clinical outcomes.

Analytical areas explored:

* Biomarker expression vs survival
* Mutation burden vs prognosis
* Hypoxia score distribution
* Stage-wise survival comparison
* Age-group survival trends

---

# Tableau Dashboard

The project includes multiple interactive Tableau dashboards for clinical and biomarker analytics.

## Dashboard 1 — Executive Overview

### KPIs

* Total Patients
* Average Diagnosis Age
* Median Survival Months
* Event Rate

### Visualizations

* Survival distribution
* Stage-wise patient count
* Age-group distribution

---

## Dashboard 2 — Biomarker Analytics

### Visualizations

* Biomarker expression comparison
* Biomarker vs survival correlation
* Expression distribution plots
* Heatmaps and comparative charts

---

## Dashboard 3 — Risk Stratification Analysis

### Visualizations

* High-risk vs low-risk survival comparison
* Stage-wise risk distribution
* Age-group risk analysis
* Kaplan-style survival trend visualization
* Treatment alignment insights

---

# Key Insights

* Biomarker expression patterns demonstrate significant variation across patient groups.
* Risk-group segmentation shows observable survival differences.
* Higher mutation burden and hypoxia scores may correlate with poorer prognosis.
* Survival outcomes vary substantially across age groups and cancer stages.
* Biomarker-driven analytics can support precision medicine and treatment planning.

---

# Tech Stack

| Category        | Tools                                   |
| --------------- | --------------------------------------- |
| Programming     | Python                                  |
| Data Processing | Pandas, NumPy                           |
| Database        | SQL                                     |
| Visualization   | Tableau                                 |
| Analytics       | Statistical Modeling, Survival Analysis |
| Domain          | Bioinformatics, Clinical Analytics      |

---

# Project Workflow

```text
Clinical Data + Expression Data
            ↓
      Data Cleaning
            ↓
      SQL Integration
            ↓
 Biomarker Analysis
            ↓
 Risk Stratification
            ↓
 Survival Analysis
            ↓
 Tableau Dashboard
            ↓
 Clinical Insights
```

# Applications

This project demonstrates practical applications in:

* Precision medicine
* Clinical decision support
* Oncology analytics
* Biomarker-based prognosis
* Healthcare data visualization
* Translational bioinformatics

---

# Learning Outcomes

Through this project, the following skills were applied:

* Clinical data analysis
* Biomarker interpretation
* SQL data modeling
* Tableau dashboard design
* Risk stratification analytics
* Exploratory statistical analysis
* Data storytelling for healthcare

---

# Author

Preeti A Sharma
Data Analytics capstone Project
Focus- Python, SQL, Tableau Dashboard and Story, Clinical Data Analytics, Biomarker-Analytics
---

# Disclaimer

This project is intended for educational and analytical purposes only. It is not designed for direct clinical diagnosis or medical decision-making.

