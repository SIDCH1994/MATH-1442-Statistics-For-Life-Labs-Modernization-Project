# 📘 Lab 08 — Hypothesis Testing  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 08 introduces **formal statistical decision-making** through hypothesis testing. Building on Lab 07’s confidence interval framework, this lab focuses on using **sample data to evaluate claims about population parameters**.

Students apply the **six-step hypothesis testing procedure** to both **population proportions** and **population means**, learning how to formulate hypotheses, select appropriate tests, compute p-values, validate assumptions, and communicate conclusions in clear, non-technical language. The lab also demonstrates how hypothesis testing can be applied to **sub-populations** using filtering, reinforcing real-world analytical reasoning.

---

## 🎯 Learning Objectives

By the end of this lab, students are able to:

- Formulate **null and alternative hypotheses** for real-world claims
- Identify the **type of hypothesis test** (left-, right-, or two-tailed)
- Conduct hypothesis tests for:
  - Population proportions
  - Population means
- Interpret **p-values** in context
- Make statistically valid decisions using a chosen significance level
- Validate hypothesis tests by checking required assumptions
- Apply hypothesis testing to **sub-groups** of a population
- Communicate conclusions in **clear, non-technical language**

---

## 📊 Statistical Concepts Covered

- Inferential statistics and decision-making
- Null hypothesis vs. alternative hypothesis
- Significance level (α)
- P-values
- One-sample binomial test for proportions
- One-sample t-test for population means
- Left-tailed, right-tailed, and two-tailed tests
- Assumption checks:
  - \( np̂ \ge 5 \) and \( nq̂ \ge 5 \) for proportions
  - Sample size and normality conditions for means
- Hypothesis testing for sub-populations
- Practical interpretation vs. statistical significance

---

## 🧰 Tools & Technology

This lab integrates hypothesis testing with modern statistical tools:

- **Jamovi**
  - Binomial tests for population proportions
  - One-sample t-tests for population means
  - Descriptive plots and Q–Q plots for assumption checking
  - Filtering for sub-group analysis
- **R (via Jamovi’s Rj Editor)**
  - Supporting calculations
  - Validation of test logic
  - Reproducible analysis using fixed random seeds
- **Python (optional / supporting)**
  - Dataset inspection and preprocessing (outside Jamovi)

---

## 📁 Dataset

### Student Survey Dataset (`SStudy.csv`)

This lab uses the **Student Survey dataset**, a comprehensive dataset describing academic, cognitive, psychological, and sleep-related characteristics of college students.

**Dataset characteristics:**
- 1,000 observations
- 23 variables
- Mix of **categorical** and **numerical** variables

**Example variables include:**
- Academic performance (GPA)
- Academic standing (class year)
- Sleep patterns (weekday and weekend sleep)
- Psychological indicators (stress, anxiety, depression)
- Lifestyle factors (alcohol use)

The dataset supports hypothesis testing for both proportions and means, as well as sub-group inference.

---

## 🔄 Conceptual Workflow

This lab emphasizes **structured statistical reasoning**:

1. **State the Claim**
   - Identify the population parameter of interest
2. **Formulate Hypotheses**
   - Define null and alternative hypotheses
3. **Choose the Test**
   - Select an appropriate test and test direction
4. **Compute the Test Statistic and P-Value**
   - Use Jamovi’s hypothesis testing tools
5. **Make a Statistical Decision**
   - Compare p-value with the significance level
6. **Validate the Test**
   - Check assumptions and sample size conditions
7. **Interpret the Results**
   - Translate statistical results into plain language

---

## 📐 GAISE Alignment

This lab aligns with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)** developed by the  
:contentReference[oaicite:1]{index=1}.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students evaluate evidence and make data-driven decisions
- **Emphasize conceptual understanding**
  - Focus on interpretation rather than mechanical testing
- **Use real data**
  - Student survey data provides realistic inferential contexts
- **Integrate technology purposefully**
  - Jamovi supports valid hypothesis testing and diagnostics
- **Foster active learning**
  - Sub-group analysis encourages exploration and reasoning
- **Prepare students for inference**
  - Builds foundations for confidence intervals and future modeling

---

## 📂 Repository Structure (Public-Safe)

```
Lab-08/
├── Data_Cleaning/
│ └── Sleep_Study.csv
│ └── data_cleaning_lab8.ipynb
├── Data_Expansion/
│ └── SStudy.csv
│ └── synthetic_data_expansion_ctgan.ipynb
├── Data_Extraction/
│ └── SStudy_Raw.csv
│ └── raw_data_extraction_lab8.ipynb
└── README.md
```

> 🔒 Full lab manuals, screenshots, assignments, and grading rubrics are intentionally excluded and maintained in a private, department-owned repository.

## 🚀 Why This Lab Matters

Hypothesis testing is central to evidence-based decision-making across disciplines. This lab helps students:

- Evaluate claims using data rather than intuition
- Understand the meaning and limitations of p-values
- Make defensible statistical decisions
- Build skills essential for research, policy analysis, and data-driven reasoning

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
