# MSc Thesis Project – Osteoarthritis Risk Prediction Using Machine Learning
End-to-end machine learning pipeline for predicting osteoarthritis risk in older adults using self-reported data from the English Longitudinal Study of Ageing (cross-sectional analysis).
# Project Description
**Academic Context:** This project was completed as part of my MSc Health Data Science degree at the University of Birmingham (2025).  
**Title:** Predicting Osteoarthritis in Older Adults Using Literature-Based, Non-Invasive Risk Factors: A Cross-Sectional Analysis of ELSA Wave 9 

## Overview
This repository contains the complete codes and results for my MSc Health Data Science thesis.  
The project develops and evaluates machine learning models to predict osteoarthritis (OA) risk in older adults using non-invasive, self-reported survey data.

## Repository Structure
- **codes/** – All data cleaning, feature selection, and modelling scripts.
- **results/** – Final outputs, including:
  - **plots/** – Visualizations such as feature importance plots and histograms.
  - **roc-curves/** – ROC curves for different models tested.
  - **tables/** – Statistical results including descriptive summaries and bivariate analysis.

## Research Objectives
- Develop predictive models estimating osteoarthritis risk in adults aged 60+ using ELSA Wave 9.
- Evaluate performance of non-invasive, literature-based risk factors.
- Assess feasibility of OA prediction without radiographic or lab-based data.
- Explore low-cost screening applications for primary care and digital health.

## Dataset
- **Source:** English Longitudinal Study of Ageing (ELSA), Wave 9 (2018–2019)
- **Sample size:** 4,723 participants aged ≥ 60 years
- **Outcome:** Self-reported osteoarthritis status
- **Predictors:** 32 literature-based, non-invasive features (reduced to 25 after feature selection)

## Methods
- Data Source: ELSA Wave 9
- Models: Logistic Regression, Random Forest, XGBoost, CatBoost
- Feature Selection: Bivariate Analysis, Boruta, Variance Inflation Factor (VIF) for Multicollinearity, Spearman correlation
- Evaluation: AUC, accuracy, presicion, recall, F1 score, confusion matrix, ROC curves

![Machine Learning Workflow](results/plots/oa_ml_workflow.png)

## Key Findings
- **Best-performing model:** Logistic Regression with upsampling (AUC: 0.755)
- **Top 15 predictors:** Difficulty stooping/kneeling, sex, pain severity (most of the time), hip pain, knee pain, age, difficulty shopping for groceries, grip strength, pain while walking, pain elsewhere, difficulty dressing, difficulty sitting for 2 hours, difficulty reaching overhead, back pain, foot pain.

## Potential Applications
- **Logistic Regression model:** Screening tool with high sensitivity for early OA detection.
- **CatBoost model:** Rule-out tool with high specificity to reduce unnecessary testing.
- **Integration:** Suitable for digital health platforms and primary care screening in resource-limited settings.

## Data Privacy
The original ELSA dataset is **not included** in this repository to maintain data confidentiality and privacy.  
All results are derived, aggregated, and anonymized.

## Author
**Tesneem Fnais** – MSc Health Data Science.  
University of Birmingham, 2025.
