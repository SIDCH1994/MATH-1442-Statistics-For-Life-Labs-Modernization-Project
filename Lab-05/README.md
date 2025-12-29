# 📘 Lab 05 — Probability Distributions  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 05 marks a key conceptual transition in the course—from describing observed data to **modeling random processes using probability distributions**. In this lab, students work with **discrete probability distributions**, focusing on how probabilities can be used to predict long-run behavior and quantify uncertainty.

Students compute the **mean (expected value)** and **standard deviation** of a discrete random variable, explore the **binomial probability distribution**, and compare results obtained through **theoretical formulas**, **computer simulation**, and **calculator-based computation**. The lab emphasizes how different tools arrive at the same probability conclusions, reinforcing both conceptual understanding and statistical confidence.

---

## 🎯 Learning Objectives

By the end of this lab, students can:

- Interpret a **discrete probability distribution**
- Compute the **mean (expected value)** of a random variable
- Compute the **standard deviation** of a probability distribution
- Identify situations modeled by a **binomial distribution**
- Calculate binomial probabilities for:
  - Exact values \( P(X = x) \)
  - Cumulative probabilities \( P(X \le x) \)
  - Probability intervals \( P(x_1 \le X \le x_2) \)
- Use **simulation** to approximate binomial probabilities
- Compare **theoretical**, **simulated**, and **calculator-based** probabilities
- Explain the **Law of Large Numbers** in the context of probability models

---

## 📊 Statistical Concepts Covered

- Discrete random variables
- Probability distributions
- Expected value (mean)
- Standard deviation of a probability model
- Binomial distribution assumptions:
  - Fixed number of trials
  - Two outcomes per trial
  - Independence
  - Constant probability of success
- Probability mass function (PMF)
- Cumulative distribution function (CDF)
- Probability intervals
- Simulation and relative frequency
- Law of Large Numbers

---

## 🧰 Tools & Technology

This lab integrates multiple approaches to probability computation:

- **Jamovi**
  - Discrete probability distributions
  - Binomial probability tables and plots
- **Jamovi Modules**
  - *saRa* module for binomial distributions and visualizations
- **R (via Jamovi’s Rj Editor)**
  - Computing expected value and standard deviation
  - Simulating binomial experiments using `rbinom()`
  - Reproducible simulation with fixed random seeds
- **Graphing Calculators (TI-83 / TI-84)**
  - Verification of binomial probability calculations

No external dataset is required for this lab.

---

## 🔄 Conceptual Workflow

This lab emphasizes **model-based statistical thinking**:

1. **Define a Probability Model**
   - Specify possible outcomes and their probabilities
2. **Summarize the Distribution**
   - Compute mean (expected value) and standard deviation
3. **Apply the Binomial Model**
   - Identify parameters \( n \) and \( p \)
4. **Compute Theoretical Probabilities**
   - Exact, cumulative, and interval probabilities
5. **Simulate Random Experiments**
   - Use large-scale simulation to approximate probabilities
6. **Compare Methods**
   - Theoretical formulas vs. simulation vs. calculator results
7. **Interpret Results**
   - Explain convergence and variability using probability concepts

---

## 📐 GAISE Alignment

This lab aligns closely with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)**.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students reason about uncertainty using probability models
- **Emphasize conceptual understanding**
  - Focus on why probability formulas work, not memorization
- **Use multiple representations**
  - Tables, formulas, plots, and simulations
- **Integrate technology purposefully**
  - Jamovi and R support exploration, not button-pushing
- **Foster active learning**
  - Simulation encourages experimentation and discovery
- **Support reproducibility**
  - Fixed random seeds reinforce transparent analysis

---

## 📂 Repository Structure (Public-Safe)
```
Lab-05/
├── R_Code_Jamovi/
│ ├── r_code_used_in_jamovi_lab5.md
│ └── r_code_used_in_jamovi_lab5.Rmd
└── README.md
```

> 🔒 Full lab manuals, screenshots, assignments, and grading rubrics are intentionally excluded and maintained in a private, department-owned repository.

## 🚀 Why This Lab Matters

Probability distributions form the foundation for statistical inference, decision-making, and predictive modeling. This lab helps students:

- Move from describing data to **predicting outcomes**
- Understand uncertainty using formal probability models
- See how theory and simulation reinforce each other
- Build intuition needed for later topics such as normal distributions and inference

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
