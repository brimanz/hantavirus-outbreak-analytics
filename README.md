# 🛡️ Clinical System for Epidemiological Control: Hantavirus 2026

An end-to-end data engineering, advanced business intelligence, and predictive analytics ecosystem built to isolate risk vectors, track exposure timelines, and support rapid executive decision-making during a simulated 2026 Hantavirus outbreak cohort ($N=20$).

---

## 🛑 The Core Problem (From Scratch)
Epidemiological crisis response teams often face highly fragmented, raw medical records during active outbreaks. Managing a cohort without strict data governance leads to critical failures: unstandardized dates break time-series tracking, demographic risks remain hidden, and delayed clinical treatments go unquantified. 

**This project solves that exact problem from scratch.** By taking a volatile raw dataset, we established a robust pipeline that transforms unvalidated rows into a centralized healthcare command center—quantifying exactly how much a single day's delay in medical triage impacts patient survival.

---

## 📁 Repository Structure
├── data/
│   └── hantavirus_PRODUCTION_READY.csv   # Cleaned, structured & standardized dataset
├── scripts/
│   └── predictive_analysis.py            # Defended ML Pipeline (LOOCV + Odds Ratio)
└── README.md                             # Comprehensive project documentation

## ⚙️ Project Pipeline & Technical Phases

### 🛠️ Phase 1: Data Engineering & Governance (Data Wrangling)
* **ISO 8601 Compliance:** Standardized structural temporal inconsistencies by converting chaotic date string metrics (`symptom_onset`, `outcome_date`, `treatment_date`, `ship_boarded`, `confirmation_date`) into clean `YYYY-MM-DD` formats, enabling precise *Time Intelligence* capabilities.
* **Feature Normalization:** Cleaned clinical logs, handled missing values, and mapped strict categorical variables (e.g., patient symptoms, gender, and specialized transmission vectors) into analytical flags.

### 📊 Phase 2: Advanced BI & Visual Storytelling (Looker Studio)
Developed an executive healthcare dashboard utilizing a high-readability **Corporate Light Theme** engineered to deliver critical situational awareness in under 30 seconds across three strategic layers:
* **Strategic Layer (Critical KPIs):** * `Total Active Cases (20)`: Real-time cohort volume monitoring.
  * `Global Mortality Rate (25%)`: Active tracking against critical institutional safety thresholds.
  * `Maximum Alert Cases (5)`: High-urgency **Red Alert** indicators isolating patients requiring immediate biocontainment.
* **Diagnostic Layer (Temporal Causal Graphics):**
  * **Epidemiological Curve:** Traces the transmission velocity based on `symptom_onset`, visually cementing the May 10th milestone as the official institutional stabilization date.
  * **Survival & Risk Scatter Plot:** Correlates age against exposure timelines, introducing a **7-Day Critical Care Cut-off Line** that proves delayed treatment drastically increases fatal outcomes.
* **Tactical Layer (Operational Logistics):**
  * **Dynamic Triage Segmentator:** Interactive filter allowing instant dashboard updates by cohort status (Alert, Chronic, Preventive, Closed).
  * **Gender Vectors Chart:** Stacked bars illustrating distinct contact channels—revealing that males contracted the virus via international flight pathways (`Aviation Proximity`) while females were linked to local domestic clusters (`Close Contact`).
  * **Geographical Bubble Map:** Coordinates global hot zones (Johannesburg, St. Helena, Ascension) for efficient transborder contact tracing.

### 🧠 Phase 3: Statistical Modeling 
* **Validation Strategy:** Replaced traditional splits with a strict **Leave-One-Out Cross-Validation (LOOCV)** process to ensure data generalizability on future incoming patient logs.
* **Risk Factor Quantification:** Computed **Odds Ratios** to translate raw predictive metrics into healthcare directives (e.g., assessing the exact percentage increase in clinical hazard per additional exposure day).

---

## 💡 Key Insights Generated
1. **The Golden 7-Day Window:** Patients triaged and treated within the first 7 days of exposure showed a 0% mortality rate, establishing a concrete operational SLA for emergency field clinics.
2. **Bifurcated Transmission Channels:** Public health spending can be optimized by splitting strategies: applying airport/aviation screening for male demographics, while deploying community-level contact tracing for female subgroups.

---

## 💻 Tech Stack & Frameworks
* **Programming Language:** Python 3.x
* **Core Libraries:** `pandas`, `numpy`
* **BI Platform:** Looker Studio (Fluid Vertical & Horizontal Layouts)
* **Methodologies:** Agile Data Sprints, Feature Engineering, Risk Odology.

---
*Developed as a benchmark portfolio project demonstrating the integration of Data Engineering, BI Architecture, and Predictive Epidemiology.*
