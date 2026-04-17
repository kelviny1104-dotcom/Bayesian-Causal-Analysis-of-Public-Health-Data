# Bayesian-Causal-Analysis-of-Public-Health-Data

Bayesian hierarchical modeling and causal inference on U.S. asthma hospitalization and PM2.5 exposure data.

## Overview
This project analyzes U.S. state-level public health data to study two related questions:

1. After accounting for sampling variability and data sparsity, what are the robust latent estimates of age-adjusted asthma hospitalization rates across U.S. states?
2. Does long-term PM2.5 exposure increase state-level asthma hospitalization rates?

The project combines Bayesian hierarchical modeling and causal inference methods to produce more stable state-level estimates and policy-relevant comparisons.

## Research Questions
### 1) Bayesian Hierarchical Modeling
Estimate the underlying age-adjusted asthma hospitalization burden across U.S. states while accounting for:
- sparse and unbalanced reporting
- measurement uncertainty
- between-state heterogeneity

### 2) Causal Inference
Evaluate whether high long-term PM2.5 exposure is associated with higher asthma hospitalization rates after adjusting for observed confounders.

## Data Sources
- U.S. Chronic Disease Indicators (CDI) 2023 Release
- CDC Environmental Public Health Tracking (PM2.5)
- Behavioral Risk Factor Surveillance System (BRFSS)
- American Community Survey (ACS)

## Methods
### Bayesian Analysis
- Bayesian hierarchical Normal-Normal model
- Partial pooling across states
- Measurement-error modeling using CDC-reported confidence intervals
- Posterior inference with weakly informative priors

### Causal Analysis
- Propensity score modeling
- Logistic regression for treatment assignment
- Propensity score subclassification
- Comparison of treated vs. control state-years under observed confounders

## Key Findings
- Bayesian partial pooling produced more stable state-level asthma hospitalization estimates despite sparse and uneven reporting.
- The analysis found meaningful between-state heterogeneity in asthma hospitalization burden.
- High long-term PM2.5 exposure was associated with higher asthma hospitalization rates.
- The estimated causal effect was about 0.8 additional asthma hospitalizations per 10,000 residents in high-exposure state-years.
