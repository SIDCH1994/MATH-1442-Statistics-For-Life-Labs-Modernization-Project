# 📘 Lab 06 — Normal Distribution & the Central Limit Theorem  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 06 focuses on the **normal probability distribution**, one of the most important models in statistics. Building on prior labs covering probability and probability distributions, this lab introduces students to assessing normality in real data, transforming variables to improve normality, and using simulation to connect theory with empirical results.

Students use **histograms and Q–Q plots** to evaluate whether variables are approximately normally distributed, apply **mathematical transformations** when normality is violated, and compute probabilities under the normal curve using both **simulation** and **theoretical methods**. The lab concludes with a simulation-based demonstration of the **Central Limit Theorem (CLT)**, showing why normal-based inference is widely applicable—even when the underlying population is not normal.

---

## 🎯 Learning Objectives

By the end of this lab, students are able to:

- Assess normality using **histograms** and **Q–Q plots**
- Interpret departures from normality graphically
- Apply **square root, logarithmic, and natural log transformations**
- Evaluate whether transformations improve normality
- Compute probabilities under the **normal distribution**
- Compare **simulated probabilities** with **theoretical probabilities**
- Explain and demonstrate the **Central Limit Theorem**
- Interpret the behavior of **sample means** versus individual observations

---

## 📊 Statistical Concepts Covered

- Normal probability distribution
- Shape, center, and spread of continuous variables
- Q–Q (quantile–quantile) plots
- Histogram + density overlays
- Mathematical transformations:
  - Square root
  - Logarithmic
  - Natural logarithm
- Z-scores and probability intervals
- Simulation of normal random variables
- Theoretical vs. empirical probability
- Central Limit Theorem:
  - Distribution of sample means
  - Relationship between population and sampling distributions

---

## 🧰 Tools & Technology

This lab integrates graphical, computational, and theoretical tools:

- **Jamovi**
  - Descriptive statistics
  - Histograms and Q–Q plots
  - Variable transformations
- **R (via Jamovi’s Rj Editor)**
  - Simulation using `rnorm()`
  - Reproducible experiments with `set.seed()`
  - Central Limit Theorem simulation
- **Graphing Calculators (TI-84 / TI-84 Plus)**
  - Verification of theoretical normal probabilities

Python notebooks may be used in the repository for dataset inspection or support, but the core analysis is conducted within Jamovi and R.

---

## 📁 Dataset

### MLB (Major League Baseball) Dataset

This lab uses a comprehensive **MLB team-level dataset** spanning multiple seasons.

**Dataset characteristics:**
- ~2,700 observations
- Mix of numerical and categorical variables
- Variables related to wins, losses, scoring, pitching, and fielding

The dataset provides realistic examples of variables that may or may not follow a normal distribution, making it well-suited for normality assessment and transformation.

---

## 🔄 Conceptual Workflow

This lab emphasizes **distributional reasoning and simulation**:

1. **Assess Normality**
   - Use histograms and Q–Q plots to evaluate distribution shape
2. **Apply Transformations**
   - Transform skewed variables and reassess normality
3. **Model with the Normal Distribution**
   - Identify mean and standard deviation
4. **Simulate Normal Data**
   - Approximate probabilities using large-scale simulation
5. **Compare with Theory**
   - Verify results using theoretical normal probabilities
6. **Demonstrate the CLT**
   - Compare original data with distributions of sample means
7. **Interpret Results**
   - Explain why normal models work broadly in statistics

---

## 📐 GAISE Alignment

This lab aligns with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)**.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students reason about distributions, not just calculations
- **Emphasize conceptual understanding**
  - Normality is evaluated visually and contextually
- **Use real data**
  - MLB data grounds abstract probability models
- **Integrate technology purposefully**
  - Jamovi and R support exploration and simulation
- **Promote active learning**
  - Students experiment with transformations and simulations
- **Build foundations for inference**
  - CLT prepares students for hypothesis testing and confidence intervals

---

## 📂 Repository Structure (Public-Safe)

```
Lab-06/
├── Data_Cleaning/
│ └── MLB.csv
│ └── data_cleaning_lab6.ipynb
├── Data_Extraction/
│ └── MLB_Raw.csv
│ └── raw_data_extraction_lab6.ipynb
├── R_Code_Jamovi/
│ └── r_code_used_in_jamovi_lab6.Rmd
│ └── r_code_used_in_jamovi_lab6.md
└── README.md
```

> 🔒 Full lab manuals, screenshots, assignments, and grading rubrics are intentionally excluded and maintained in a private, department-owned repository.


## 🚀 Why This Lab Matters

The normal distribution and the Central Limit Theorem underpin nearly all classical statistical inference. This lab helps students:

- Understand when normal models are appropriate
- Learn how to diagnose and correct non-normality
- See why sample means behave predictably
- Build intuition essential for inference, confidence intervals, and hypothesis testing

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

