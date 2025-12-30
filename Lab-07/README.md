# 📘 Lab 07 — Confidence Intervals & Estimating Population Parameters  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 07 marks the course’s transition from descriptive statistics and probability models to **inferential statistics**. In this lab, students learn how to use **confidence intervals** to estimate unknown population parameters using sample data.

Students construct and interpret confidence intervals for **population proportions** and **population means**, examine how confidence level affects interval width, and assess whether conditions for inference are met. The lab also introduces **simulation-based reasoning** to clarify the meaning of a confidence level as a long-run success rate rather than a probability statement about a single interval.

---

## 🎯 Learning Objectives

By the end of this lab, students are able to:

- Construct and interpret confidence intervals for **population proportions**
- Construct and interpret confidence intervals for **population means**
- Compute confidence intervals using:
  - Raw data
  - Summary statistics
- Construct confidence intervals for means **separated by a categorical variable**
- Assess validity conditions for confidence intervals:
  - \( np̂ \ge 5 \) and \( nq̂ \ge 5 \) for proportions
  - \( n > 30 \) or approximate normality for means
- Interpret the meaning of a **confidence level**
- Use **simulation** to demonstrate long-run confidence interval behavior

---

## 📊 Statistical Concepts Covered

- Inferential statistics
- Population parameters vs. sample statistics
- Confidence intervals for proportions
- Confidence intervals for means
- Confidence level (90%, 95%, 99%)
- Margin of error
- Conditions for inference:
  - Normal approximation for proportions
  - Sample size and normality assumptions for means
- Confidence intervals for two groups
- Interpretation vs. misinterpretation of confidence intervals
- Repeated sampling and long-run frequency interpretation

---

## 🧰 Tools & Technology

This lab integrates inferential reasoning with modern statistical tools:

- **Jamovi**
  - Construction of confidence intervals
  - Visualization of interval estimates
  - Group comparisons using categorical variables
- **Jamovi Module**
  - *esci* (Estimation Statistics with Confidence Intervals)
- **R (via Jamovi’s Rj Editor)**
  - Simulation of repeated sampling
  - Visualization of confidence interval coverage
  - Reproducible analysis using fixed random seeds
- **Python (optional / supporting)**
  - Dataset inspection and preparation (outside Jamovi)

---

## 📁 Dataset

### Nutrition Dataset

This lab uses the **Nutrition dataset**, a cross-sectional study containing nutrition and health information for 315 individuals.

**Dataset characteristics:**
- 315 observations
- Mix of **numerical** and **categorical** variables
- Variables related to diet, smoking behavior, vitamin use, and health indicators

The dataset supports:
- Confidence intervals for proportions (categorical variables)
- Confidence intervals for means (numerical variables)
- Group comparisons based on categorical factors

---

## 🔄 Conceptual Workflow

This lab emphasizes **inferential reasoning and validation**:

1. **Select a Parameter of Interest**
   - Proportion or mean
2. **Draw a Random Sample**
   - Ensure representativeness
3. **Construct a Confidence Interval**
   - Choose confidence level
4. **Validate Conditions**
   - Check assumptions for inference
5. **Interpret the Interval**
   - Explain results in context
6. **Compare Confidence Levels**
   - Observe effects on interval width
7. **Simulate Repeated Sampling**
   - Interpret confidence level as a long-run property

---

## 📐 GAISE Alignment

This lab aligns with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)** developed by the  
:contentReference[oaicite:1]{index=1}.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students reason from samples to populations
- **Emphasize conceptual understanding**
  - Confidence intervals interpreted conceptually, not mechanically
- **Use real data**
  - Nutrition data provides realistic inferential contexts
- **Integrate technology purposefully**
  - Jamovi and R support estimation and simulation
- **Foster active learning**
  - Simulation reinforces long-run interpretation
- **Build foundations for inference**
  - Prepares students for hypothesis testing and sample size planning

---

## 📂 Repository Structure (Public-Safe)

```
├── Data_Cleaning/
│ └── Nutrition.csv
│ └── data_cleaning_lab7.ipynb
├── Data_Extraction/
│ └── Nutrition_Raw.csv
│ └── raw_data_extraction_lab7.ipynb
├── R_Code_Jamovi/
│ ├── r_code_used_in_jamovi_lab7_files/figure-gfm
|   └── unnamed-chunk-1-1.png
│ └── r_code_used_in_jamovi_lab7.Rmd
│ └── r_code_used_in_jamovi_lab7.md
└── README.md
```
r_code_used_in_jamovi_lab7_files/figure-gfm

> 🔒 Full lab manuals, screenshots, assignments, and grading rubrics are intentionally excluded and maintained in a private, department-owned repository.

---

## 🚀 Why This Lab Matters

Confidence intervals are among the most widely used tools in applied statistics. This lab helps students:

- Move from point estimates to **ranges of plausible values**
- Understand uncertainty in real-world decision-making
- Interpret confidence levels correctly
- Build intuition needed for hypothesis testing and sample size determination

---

## 🏷️ Authorship & Attribution

### Authors: 

1. **Siddhartha Chilukuri** - Graduate Research Assistant - Department of Mathematics & Statistics - Texas A&M University – Corpus Christi
<br><br>

2. **Haekyoung Choi** - Senior Instructor - Department of Mathematics & Statistics - Texas A&M University – Corpus Christi
<br><br>

3. **Dr. Jose Guardiola** - Professor - Department of Mathematics & Statistics - Texas A&M University – Corpus Christi
<br><br>

The authors contributed to the design and development of this project. This project was funded and supported by the Department of Mathematics & Statistics at Texas A&M University–Corpus Christi. All instructional materials and lab manuals associated with this project are the intellectual property of the Department. Public materials in this repository are shared for demonstration and educational purposes only.



*This README is designed for public sharing, instructional transparency, and recruiter-facing clarity. Proprietary instructional materials are excluded by design.*


