# Trichomonas vaginalis Prevalence, Risk Factors, and Diagnostic Performance Among Female Sex Workers in Lomé, Togo

## Overview

This repository contains the reproducible statistical analysis used to estimate the prevalence of *Trichomonas vaginalis* infection, identify associated risk factors, and evaluate the diagnostic performance of wet mount microscopy compared with PCR among female sex workers (FSWs) in Lomé, Togo.

The analysis was conducted using R and implemented through a fully reproducible RMarkdown workflow.

---

## Study Objectives

This analysis aimed to:

1. Estimate the prevalence of *Trichomonas vaginalis* infection among female sex workers in Lomé.
2. Identify sociodemographic, behavioral, clinical, and biological factors associated with infection.
3. Evaluate the diagnostic performance of wet mount microscopy compared with PCR.

---

## Study Design

Cross-sectional epidemiological study conducted among female sex workers in Lomé, Togo.

Participants underwent:

- Structured interviews collecting sociodemographic and behavioral data
- Clinical examination
- Laboratory testing for sexually transmitted infections

Laboratory testing included:

- Wet mount microscopy
- PCR detection of *Trichomonas vaginalis*
- Testing for other STIs including:
  - HIV
  - *Chlamydia trachomatis*
  - *Neisseria gonorrhoeae*
  - *Gardnerella vaginalis*

---

## Statistical Methods

All analyses were conducted in **R** using reproducible workflows.

The analytical pipeline included:

- Data import and cleaning
- Variable recoding and dataset preparation
- Descriptive epidemiological analysis
- Prevalence estimation with 95% confidence intervals
- Bivariate association analysis using Chi-square and Fisher’s exact tests
- Univariable logistic regression
- Multivariable logistic regression with stepwise model selection (AIC)
- Model diagnostics:
  - Hosmer–Lemeshow goodness-of-fit test
  - Variance Inflation Factor (VIF)
- Diagnostic test evaluation:
  - McNemar test
  - Cohen’s Kappa coefficient
  - Sensitivity, specificity, predictive values, likelihood ratios

---

## Key Results

- Overall prevalence of *Trichomonas vaginalis*: **14.0% (95% CI: 10.7–18.1)**.
- Prevalence varied across participant characteristics.
- *Gardnerella vaginalis* infection was significantly associated with *Trichomonas vaginalis* infection in bivariate analysis.
- Multivariable logistic regression identified several independent factors associated with infection.
- Wet mount microscopy showed **low sensitivity (24%)** compared with PCR.

---

## Repository Structure


---

## Data Availability

Due to confidentiality agreements with the study institution, the dataset used in this analysis cannot be publicly shared.

The repository therefore provides:

- The complete analytical workflow (RMarkdown)
- The rendered analysis report (HTML)

This allows full transparency of the statistical methods and analytical procedures.

---

## Reproducibility

To render the analysis report locally:

```r
rmarkdown::render("tv_analysis_fsw_lome.Rmd")
