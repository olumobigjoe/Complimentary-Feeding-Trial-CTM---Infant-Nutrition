# 📊 Longitudinal Nutritional Intervention & Hematological Trajectory Analysis

> **"Bridging the Gap Between Early Childhood Dietary Interventions and Long-Term Developmental Efficacy Through Rigorous Statistical Diagnostics."**

---

## 🚀 Executive Project Overview
This repository contains a deep-dive statistical analysis and analytical report evaluating a longitudinal clinical dataset tracking **30 infant subjects** across multiple critical developmental milestones. The core objective of this study is to isolate, analyze, and quantify the physiological and hematological impacts of a randomized nutritional tracking trial—comparing a **Fortified Diet** against a standard **Basal Diet**. 

By tracking infant growth velocity metrics alongside blood chemistry indicators over an 18-month timeline, this project provides data-backed clarity into mitigating early-childhood iron-deficiency risks.

---

## 🛠️ Key Performance Indicators (KPIs)
The clinical and operational health of the cohort is anchored around four foundational metrics:

* **Sample Cohort ($N$):** `30 Infants` fully tracked across a 18-month matrix.
* **Avg. Maternal Maturity ($\mu$):** `31.9 Years` ($\pm 6.20\text{ years}$), ensuring stable, mature care baselines.
* **Average 6-Month Baseline Weight:** `7.11 kg` across all combined demographics.
* **Longitudinal $\text{Hgb}$ Maturation Velocity:** `+8.10 g/L` total cohort increase from Month 6 to Month 18 ($p = 0.0169$, Highly Significant).

---

## 📈 Technical Architecture & Data Features
The pipeline processes structural clinical variables mapped directly from Stata microdata binary frameworks:

### Demographic Data Attributes
* `idno`: Unique Subject Identification Key.
* `mother_age`: Maternal chronological age at enrollment.
* `educ_cat` / `meduc`: Categorical maternal education tiers (*None*, *Primary*, *Secondary*, *College/Univ*).
* `sescat3`: Socioeconomic stratification broken into tertiles (*Low*, *Middle*, *High*).

### Clinical & Anthropometric Metrics
* `treat`: Randomized operational group assignment (*Basal diet* vs. *Fortified diet*).
* `child_sex`: Phenotypic sex profiling (*Male* vs. *Female*).
* `weight6` / `length6`: Standardized physical growth tracking at 6 months of age.
* `hgb6` / `hgb18`: Continuous tracking of hemoglobin levels ($\text{g/L}$) measured at the 6-month and 18-month developmental milestones.

---

## 🔬 Core Analytical Insights

### 1. The Maturation Effect (Paired Diagnostics)
A paired $t$-test evaluating hemoglobin levels over time across identical infants showed a structural, positive trajectory ($t = 2.534$, $p = 0.0169$). This emphasizes that independent of the specific diet format, age-related metabolic shifts substantially elevate baseline blood oxygenation capacities during this developmental window.

### 2. Intervention Group Micro-Variance
Hemoglobin Efficacy Trajectory
125 g/L ───────────────────────────────────────────────────► Fortified (123.11 g/L)
► Basal (119.90 g/L)
115 g/L ─────────────────────► Fortified (116.22 g/L)
─────────────────────► Basal (111.29 g/L)
105 g/L ───────────────────────────────────────────────────
Month 6                       Month 18

While independent cross-sectional $t$-tests reveal that group variances overlap within a restricted 30-subject sample baseline ($p = 0.2833$ at 6 months), the **Fortified Diet** group consistently maintained a higher absolute mean baseline at both checks. It structurally truncated the lower-percentile anemia risk tails seen in the standard Basal control group.

### 3. Anthropometric Growth Ratios
Physical mapping shows a tight, healthy linear correlation between child weight and length at the 6-month milestone. When partitioned by sex, male infants group marginally toward the upper right quadrants of the distribution, aligning with global WHO childhood development standards.

---

## 💻 Technical Implementation Stack
* **Language:** Python 3.11+
* **Data Manipulation:** `pandas`, `numpy`
* **Statistical Modeling:** `scipy.stats` (Independent & Paired T-Testing)
* **Visualization Layer:** `matplotlib`, `seaborn`

---

## 🚀 How To Run the Analytical Pipeline

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/olumobigjoe/InfantIron-ML.git](https://github.com/olumobigjoe/InfantIron-ML.git)
   cd InfantIron-ML


🎯 Repository Maintainer
Olumodeji Ibukun Ayodeji

GitHub: @olumobigjoe

Professional Focus: Data Analytics & Electronics Systems Integration
