# 📘 Lab 09 — Two-Sample Hypothesis Testing  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 09 extends hypothesis testing to situations involving **two populations or two conditions**, completing the inferential framework introduced in Labs 07 and 08. While earlier labs focused on inference for a single population, this lab addresses one of the most common real-world questions in statistics: **Are two groups meaningfully different?**

Students apply hypothesis testing procedures to compare **two independent population means** and **two dependent (paired) population means** using appropriate t-tests. The lab emphasizes **test selection based on study design**, **assumption validation**, and **clear, non-technical interpretation of results**.

---

## 🎯 Learning Objectives

By the end of this lab, students are able to:

- Distinguish between **independent** and **dependent (paired)** samples
- Select the appropriate two-sample hypothesis test based on study design
- Perform and interpret an **Independent Samples t-Test**
- Perform and interpret a **Paired Samples t-Test**
- Formulate correct null and alternative hypotheses for two-sample tests
- Identify test direction (left-, right-, or two-tailed)
- Validate hypothesis tests by checking required assumptions
- Communicate statistical conclusions in **clear, non-technical language**

---

## 📊 Statistical Concepts Covered

- Two-sample inference
- Independent vs. dependent samples
- Population mean comparison
- Independent Samples t-Test
- Paired Samples t-Test
- Mean difference (\( \mu_1 - \mu_2 \), \( \mu_d \))
- Hypothesis formulation for two samples
- Significance level (α) and p-values
- One-tailed vs. two-tailed tests
- Assumption checks:
  - Sample size conditions
  - Normality of distributions or differences
  - Homogeneity of variances (independent samples)
- Practical vs. statistical significance

---

## 🧰 Tools & Technology

This lab integrates inferential reasoning with modern statistical tools:

- **Jamovi**
  - Independent Samples t-Tests
  - Paired Samples t-Tests
  - Confidence interval plots
  - Q–Q plots for assumption checking
  - Filtering for random sampling and subgroup analysis
- **R (via Jamovi’s Rj Editor)**
  - Validation of test logic
  - Supporting calculations and reproducibility
- **Python (optional / supporting)**
  - Dataset inspection and preprocessing (outside Jamovi)

---

## 📁 Datasets

### ICU Admissions Dataset (`ICUAdmissions.csv`)

Used for **independent samples hypothesis testing**.

**Dataset characteristics:**
- 1,200 observations
- Mix of **categorical** and **numerical** variables
- Patient demographics, admission characteristics, and vital signs

Example use:
- Comparing mean heart rate between **male and female** patients

---

### Forest Restoration Dataset (`Forest_Restoration.csv`)

Used for **paired samples hypothesis testing**.

**Dataset characteristics:**
- 1,000 observations
- Measurements taken **before and after** a restoration treatment
- Ecological indicators such as biomass, soil moisture, and temperature

Example use:
- Comparing **pre-treatment vs. post-treatment** biomass levels

---

## 🔄 Conceptual Workflow

This lab emphasizes **study design–driven inference**:

1. **Identify the Research Question**
   - Are two groups independent or paired?
2. **Select the Appropriate Test**
   - Independent or Paired Samples t-Test
3. **Formulate Hypotheses**
   - Define null and alternative hypotheses
4. **Choose Test Direction**
   - Left-tailed, right-tailed, or two-tailed
5. **Compute Test Statistic and P-Value**
   - Use Jamovi’s hypothesis testing tools
6. **Make a Statistical Decision**
   - Compare p-value with α
7. **Validate Assumptions**
   - Check sample size and normality conditions
8. **Interpret Results**
   - Translate statistical findings into plain language

---

## 📐 GAISE Alignment

This lab aligns with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)** developed by the  
:contentReference[oaicite:1]{index=1}.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students reason about differences between groups
- **Emphasize conceptual understanding**
  - Focus on test selection and interpretation, not mechanics
- **Use real data**
  - Clinical and ecological datasets provide authentic contexts
- **Integrate technology purposefully**
  - Jamovi supports valid inference and diagnostics
- **Foster active learning**
  - Students evaluate multiple claims and study designs
- **Complete the inferential cycle**
  - Builds on confidence intervals and one-sample testing

---

## 📂 Repository Structure (Public-Safe)
```
Lab-09/
├── Data_Dependent_Sample/
│ ├── Data_Cleaning/
│ │ ├── Forest_Restoration.csv
│ │ └── data_cleaning_lab9_D_sample.ipynb
│ ├── Data_Generation/
│ │ ├── Forest_Study_Raw.csv
│ │ └── synthetic_data_generation_lab9.ipynb
├── Data_Independent_Sample/
│ ├── Data_Cleaning/
│ │ ├── ICU_Cleaned.csv
│ │ └── data_cleaning_lab9_ID_sample.ipynb
│ ├── Data_Expansion/
│ │ ├── ICUAdmissions.csv
│ │ ├── ICU_Expanded_Raw.csv
│ │ └── synthetic_data_expansion_smoteec.ipynb
│ ├── Data_Extraction/
│ │ ├── ICU_Admissions_Raw.csv
│ │ └── raw_data_extraction_lab9_ID_sample.ipynb
└── README.md
```


> 🔒 Full lab manuals, screenshots, assignments, and grading rubrics are intentionally excluded and maintained in a private, department-owned repository.


## 🚀 Why This Lab Matters

Two-sample hypothesis testing is central to scientific comparison and evidence-based decision-making. This lab helps students:

- Choose the correct tests based on the study design
- Avoid common misapplications of statistical tests
- Interpret results responsibly and clearly
- Apply inferential reasoning to real-world comparisons

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


*This README is designed for public sharing, instructional transparency, and professional presentation. Proprietary instructional materials are excluded by design.*

