# 📘 Lab 04 — Probability & Simulation  
**MATH 1442: Statistics for Life**

---

## 🔍 Lab Overview

Lab 04 introduces students to **probability as a tool for modeling uncertainty and predicting outcomes**. Building on earlier labs that focused on describing and comparing observed data, this lab shifts attention toward **theoretical probability, compound events, and long-run behavior of random processes**.

Students compute probabilities using **frequency tables** and **contingency tables**, then explore how probability behaves in practice through **simulation**. Using Jamovi’s integration with R, students design and run numerical experiments that illustrate the **Law of Large Numbers**, reinforcing the connection between theoretical probability and empirical results.

---

## 🎯 Learning Objectives

By the end of this lab, students are able to:

- Compute probabilities from **frequency tables**
- Use **contingency tables** to calculate:
  - AND probabilities
  - OR probabilities
  - Complement probabilities
  - Conditional probabilities
- Interpret probabilities in real-world contexts
- Use **simulation** to model random processes
- Explain the **Law of Large Numbers**
- Compare **theoretical probabilities** with **simulated results**
- Understand the role of **reproducibility** in simulation using random seeds

---

## 📊 Statistical Concepts Covered

- Sample space and events
- Classical probability
- Relative frequency interpretation
- Frequency tables and proportions
- Contingency tables
- Compound events:
  - Intersection (AND)
  - Union (OR)
  - Complement (NOT)
  - Conditional probability
- Simulation and randomness
- Law of Large Numbers
- Empirical vs. theoretical probability

---

## 🧰 Tools & Technology

This lab integrates graphical analysis with computational thinking:

- **Jamovi**
  - Frequency tables
  - Contingency tables
  - Probability interpretation using real datasets
- **R (via Jamovi’s R editor)**
  - Simulation of random experiments
  - Reproducible analysis using `set.seed()`
- **Python (optional / supporting)**
  - Dataset inspection and preparation (outside Jamovi)
  - Reinforces transferable data-science workflows

No prior programming experience is required.

---

## 📁 Datasets

### Ames Housing Dataset
Students use the **Ames Housing dataset**, a widely cited real-world dataset describing residential properties in Ames, Iowa.

**Key features:**
- ~2,700 observations
- Mix of **categorical and numerical variables**
- Housing characteristics such as building type, roof style, utilities, and sale conditions

This dataset allows probability concepts to be grounded in a realistic decision-making context.

### Simulated Data
Students also generate **synthetic data** through simulation to model:
- Rolling a fair six-sided die
- Drawing cards from a single suit

These simulations provide controlled environments for studying probability behavior.

---

## 🔄 Conceptual Workflow

This lab emphasizes **probability reasoning**, not memorization:

1. **Observed Data**
   - Use frequency tables to estimate probabilities
2. **Compound Events**
   - Compute AND, OR, complement, and conditional probabilities
3. **Modeling Randomness**
   - Design simulations using R
4. **Repetition & Scale**
   - Run experiments with increasing numbers of trials
5. **Convergence**
   - Compare empirical results to theoretical probabilities
6. **Interpretation**
   - Explain why results stabilize as trials increase

---

## 📐 GAISE Alignment

This lab aligns with the **Guidelines for Assessment and Instruction in Statistics Education (GAISE)** developed by the  
:contentReference[oaicite:1]{index=1}.

### GAISE Principles Addressed

- **Teach statistical thinking**
  - Students reason about uncertainty and long-run behavior
- **Emphasize conceptual understanding**
  - Probability rules are interpreted through data and simulation
- **Use real data**
  - Housing data provides realistic probability contexts
- **Integrate technology purposefully**
  - Jamovi and R are used to explore ideas, not replace reasoning
- **Promote active learning**
  - Simulation allows experimentation and discovery
- **Support reproducibility**
  - Random seeds highlight transparent, repeatable analysis

---

## 📂 Repository Structure (Public-Safe)
```
Lab-04/
├── Data_Cleaning/
│ └── Ames_Housing.csv
│ └── data_cleaning_lab4.ipynb
├── Data_Extraction/
│ └── Ames_Housing_Raw.csv
│ └── raw_data_extraction_lab4.ipynb
├── R_Code_Jamovi/
│ └── r_code_used)in_jamovi_lab4.Rmd
│ └── r_code_used)in_jamovi_lab4.md
└── README.md
```


🔒 Full lab manuals, screenshots, step-by-step instructions, and grading rubrics are maintained separately in a private, department-owned repository.

---

## 🚀 Why This Lab Matters

Probability underpins decision-making in science, business, health, and everyday life. This lab helps students:

- Develop intuition for uncertainty
- Understand how probabilities behave in the long run
- See how simulation supports real-world modeling
- Build transferable skills used in data science and analytics

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









