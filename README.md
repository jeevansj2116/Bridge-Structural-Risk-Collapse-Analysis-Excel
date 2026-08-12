# 🌉 Bridge Structural Risk & Collapse Analysis | Excel

## 📌 Project Overview

**Bridge Structural Risk & Collapse Analysis** is an Excel-based data analytics project developed to analyze bridge structural conditions, collapse patterns, risk levels, and maintenance priorities across **10,000 bridge records**.

The project transforms raw bridge data into a cleaned analytical dataset and applies a structured **risk-scoring model** to identify bridges requiring enhanced inspection, priority maintenance, or immediate intervention.

---

## 🎯 Business Objective

The main objective of this project is to answer:

* What factors are associated with bridge collapse?
* How does structural stress affect collapse risk?
* How does strain vary between collapsed and standing bridges?
* Does bridge age contribute to vulnerability?
* How do traffic volume and environmental conditions relate to collapse?
* Which bridges should receive maintenance priority?
* Which risk levels contain the highest proportion of collapsed bridges?

---

# 📂 Project Files

```text
Bridge-Structural-Risk-Analysis/
│
├── README.md
│
├── data/
│   ├── Bridge_Data_Raw.xlsx
│   └── Bridge_Data_Cleaned.xlsx
│
├── analysis/
│   └── Bridge_Data_Analysis.xlsx
│
└── screenshots/
    ├── risk_model.png
    ├── summary_statistics.png
    ├── pivot_analysis.png
    └── maintenance_tracker.png
```

### File descriptions

**Bridge_Data_Raw.xlsx**
Contains the original 10,000 bridge records and structural/environmental variables.

**Bridge_Data_Cleaned.xlsx**
Contains the cleaned analytical dataset.

**Bridge_Data_Analysis.xlsx**
Contains the main analysis including:

* Maintenance Priority Tracker
* Risk Scoring Model
* Summary Statistics
* Pivot Analysis

---

# 📊 Dataset

The dataset contains bridge-level information such as:

* Bridge ID
* Location
* Age
* Material
* Length
* Width
* Height
* Traffic Volume
* Weather Conditions
* Water Flow Rate
* Maintenance History
* Stress
* Strain
* Tensile Strength
* Rainfall
* Material Composition
* Bridge Design
* Construction Quality
* Temperature
* Humidity
* Collapse Status
* Age Group
* Risk Score
* Risk Level
* Collapse Flag

---

# 🧹 Data Preparation

The project follows a simple:

```text
Raw Data
   ↓
Data Cleaning
   ↓
Risk Scoring
   ↓
Statistical Analysis
   ↓
Pivot Analysis
   ↓
Maintenance Prioritization
```

The cleaned workbook preserves the bridge-level variables while preparing the data for analysis.

---

# ⚠️ Structural Risk Scoring Model

A composite **Risk Score** is used to classify bridge risk.

The scoring model uses three major components:

| Risk Component          | Weight |
| ----------------------- | -----: |
| Structural Stress Index |    40% |
| Strain Risk Index       |    30% |
| Age Vulnerability Index |    30% |

The model uses:

```text
Structural Stress Index
= Stress / Maximum Stress × 40

Strain Risk Index
= Strain / Maximum Strain × 30

Age Vulnerability Index
= Age / 50 × 30
```

The scoring parameters and formula basis are defined in the project's Risk Scoring Model.

---

# 🚦 Risk Classification

The project classifies bridges into four risk categories:

| Risk Level  | Score Range | Recommended Action     |
| ----------- | ----------: | ---------------------- |
| 🟢 Low      |        0–30 | Routine monitoring     |
| 🟡 Moderate |       31–55 | Enhanced inspection    |
| 🟠 High     |       56–75 | Priority maintenance   |
| 🔴 Critical |      76–100 | Immediate intervention |

These thresholds and actions are defined directly in the analysis workbook.

---

# 📈 Key Results

The analysis contains **10,000 bridges**:

* **2,000 collapsed**
* **8,000 standing**
* **20% overall collapse rate**
* **49.7 average risk score**
* **24.5 years average bridge age**

The summary analysis reports these as the primary project-level metrics.

---

# 🔍 Collapse Analysis

## By Material

| Material | Total | Collapsed | Standing | Collapse Rate |
| -------- | ----: | --------: | -------: | ------------: |
| Concrete | 3,333 |       666 |    2,667 |         20.0% |
| Steel    | 3,334 |       667 |    2,667 |         20.0% |
| Wood     | 3,333 |       667 |    2,666 |         20.0% |

The material-level results show very similar collapse rates across the three materials.

---

## By Bridge Design

| Design | Total | Collapsed | Standing | Collapse Rate |
| ------ | ----: | --------: | -------: | ------------: |
| Arch   | 3,334 |       667 |    2,667 |         20.0% |
| Beam   | 3,333 |       666 |    2,667 |         20.0% |
| Truss  | 3,333 |       667 |    2,666 |         20.0% |

---

## By Region

The dataset contains five regions:

* Region 1
* Region 2
* Region 3
* Region 4
* Region 5

Each region contains 2,000 bridges, with 400 collapsed bridges, producing a 20% collapse rate in each region.

---

# 👴 Age Group Analysis

The project analyzes collapse by bridge age.

| Age Group | Total | Collapsed | Collapse Rate |
| --------- | ----: | --------: | ------------: |
| 0–10 yrs  | 2,227 |       456 |         20.5% |
| 11–20 yrs | 1,979 |       375 |         18.9% |
| 21–30 yrs | 1,944 |       380 |         19.5% |
| 31–40 yrs | 2,037 |       391 |         19.2% |
| 41–50 yrs | 1,813 |       398 |         22.0% |

The **41–50 year** group has the highest reported collapse rate at approximately **22%**.

---

# 🌦️ Weather Analysis

Collapse patterns were also analyzed across:

* Cloudy
* Rainy
* Snowy
* Sunny
* Windy

The summary analysis reports a 20% collapse rate for each weather category.

This suggests that, within this dataset, weather category alone does not distinguish the collapse groups.

---

# 📊 Risk Level Distribution

| Risk Level | Count | Collapsed | Collapse Rate |
| ---------- | ----: | --------: | ------------: |
| Low        | 2,256 |         0 |            0% |
| Moderate   | 3,484 |         0 |            0% |
| High       | 2,789 |       806 |         28.9% |
| Critical   | 1,471 |     1,194 |         81.2% |

### Key observation

The **Critical** category contains the strongest concentration of collapsed bridges:

**1,194 of 1,471 critical-risk bridges are classified as collapsed**, corresponding to an **81.2% collapse rate**.

The High-risk category has a 28.9% collapse rate.

This makes the risk score particularly useful for maintenance prioritization.

---

# 📌 Collapsed vs Standing Comparison

The analysis compares important structural and environmental indicators.

| Metric          | Collapsed Avg. | Standing Avg. | Difference |
| --------------- | -------------: | ------------: | ---------: |
| Stress          |         90 MPa |        40 MPa | +50.01 MPa |
| Strain          |             9% |            4% |        +5% |
| Age             |      24.85 yrs |     24.39 yrs |  +0.46 yrs |
| Traffic Volume  |        9,010.4 |       4,059.9 |   +4,950.5 |
| Rainfall        |      450.02 mm |     199.99 mm | +250.03 mm |
| Temperature     |           42°C |           2°C |      +40°C |
| Humidity        |            90% |           40% |    +50.01% |
| Water Flow Rate |   4,500.2 m³/s | 1,999.95 m³/s |  +2,500.25 |
| Risk Score      |          77.91 |         42.63 |     +35.28 |

These are descriptive comparisons from the dataset and should be interpreted as **associations, not proof of causation**.

---

# 🔄 Multi-Dimensional Pivot Analysis

The project uses pivot analysis to examine combinations of variables.

### Pivot 1

**Material × Bridge Design**

Used to analyze collapse counts across combinations such as:

* Concrete × Beam
* Steel × Arch
* Wood × Truss

### Pivot 2

**Region × Weather**

Used to examine collapse rates across geographic and weather combinations.

### Pivot 3

**Age Group × Material**

Used to compare average risk scores across bridge age groups and materials.

The pivot analysis shows that average risk score increases across the age groups, from approximately **37.9 for 0–10 years** to **63.1 for 41–50 years**.

---

# 🛠️ Maintenance Priority Tracker

A dedicated **Maintenance Priority Tracker** was created for bridges classified as **Critical or High Risk**.

The tracker includes:

* Bridge ID
* Location
* Material
* Design
* Age
* Stress
* Strain
* Risk Score
* Risk Level
* Weather
* Collapse Status
* Last Maintenance Date

This allows high-risk bridges to be prioritized for inspection and intervention.

---

# 📌 Business Insights

### 1. Risk score is strongly associated with collapse status

Critical-risk bridges show a substantially higher collapse rate than Low and Moderate risk groups.

### 2. Structural stress is a major differentiator

Average stress is considerably higher among collapsed bridges than standing bridges.

### 3. Strain is also substantially higher

Collapsed bridges show a higher average strain compared with standing bridges.

### 4. Traffic volume differs substantially

Collapsed bridges have a much higher average traffic volume in this dataset.

### 5. Older bridges show higher risk scores

Average risk score rises across the age groups, supporting age as an important component of the scoring framework.

### 6. Maintenance prioritization

The risk classification can be used to prioritize inspection and maintenance resources toward High and Critical bridges.

---

# 🧰 Excel Skills Demonstrated

### Data Cleaning

* Data validation
* Data preparation
* Handling structured datasets
* Creating analytical datasets

### Data Analysis

* Descriptive statistics
* Group-wise analysis
* Risk scoring
* Comparative analysis
* Collapse-rate analysis

### Excel Analytics

* Pivot Tables
* Multi-dimensional analysis
* Summary statistics
* Conditional analysis
* Maintenance tracking

### Risk Analytics

* Composite risk scoring
* Risk classification
* Risk-based prioritization
* Structural risk assessment

---

# 📁 Recommended Repository Structure

```text
Bridge-Structural-Risk-Analysis/
│
├── README.md
│
├── data/
│   ├── Bridge_Data_Raw.xlsx
│   └── Bridge_Data_Cleaned.xlsx
│
├── analysis/
│   └── Bridge_Data_Analysis.xlsx
│
└── screenshots/
    ├── risk_scoring_model.png
    ├── summary_statistics.png
    ├── pivot_analysis.png
    └── maintenance_tracker.png
```

---

# 🚀 Project Workflow

```text
10,000 Raw Bridge Records
          ↓
   Data Preparation
          ↓
    Cleaned Dataset
          ↓
  Risk Score Calculation
          ↓
 Risk Level Classification
          ↓
 Summary Statistics
          ↓
  Pivot Analysis
          ↓
Maintenance Prioritization
```

---

# 🎓 Learning Outcomes

This project demonstrates the ability to:

* Work with a large structured dataset in Excel
* Clean and prepare data for analysis
* Build a composite risk-scoring framework
* Perform descriptive and comparative analysis
* Use Pivot Tables for multi-dimensional analysis
* Identify high-risk records
* Translate analytical results into maintenance priorities
* Present data-driven findings for infrastructure management

---

## 👤 Author

**Jeevan**

 Data Analyst | SQL | Python | Power BI | Excel | AI-ML | Machine Learning | business Intelligence

---



