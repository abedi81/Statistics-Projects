# Survival Analysis Using Weibull Distribution

## Overview

This project applies survival analysis techniques to study system reliability using simulated time-to-event data.

The goal is to model how failure risk evolves over time and to extract meaningful reliability metrics that can support engineering and decision-making processes.

A Weibull distribution is used as the underlying model due to its flexibility in capturing different failure behaviors.

---

## Problem Setup

A realistic dataset is generated to mimic a reliability scenario:

- Each unit has a true failure time drawn from a Weibull process  
- Some observations are randomly censored  
- The dataset includes:
  - Observed time  
  - Event indicator (failure or censored)  

 This setup reflects real-world survival data where not all failures are observed.

---

## Methodology

The analysis follows a structured survival modeling approach:

1. Simulate time-to-event data with censoring  
2. Define observed time and event indicators  
3. Fit a parametric Weibull model  
4. Estimate distribution parameters  
5. Derive survival and hazard-related functions  
6. Compute reliability metrics  
7. Validate model fit  

---

## Key Concepts

The project explores core survival analysis components:

- **Survival Function (S(t))** → Probability of surviving beyond time t  
- **Hazard Function (h(t))** → Instantaneous failure risk  
- **Cumulative Hazard** → Accumulated risk over time  

 These functions describe how failure risk evolves.

---

## Reliability Metrics

Several practical reliability measures are computed:

- **Mean Time to Failure (MTTF)**  
- **Median Survival Time**  
- **B-life metrics (B10, B50, B90)**  

 These metrics are widely used in engineering, warranty design, and risk assessment.

---

## Visualization

The model is interpreted using multiple plots:

- Probability density function (failure distribution)  
- Survival curve  
- Hazard function  
- Cumulative hazard  

 These visualizations provide intuition about failure patterns and risk accumulation.

---

## Practical Insights

The model is translated into actionable insights:

- Probability of surviving a warranty period  
- Conditional survival probabilities  
- Risk evolution over time  

 This connects statistical modeling to real-world decision-making.

---

## Model Validation

Model fit is evaluated using:

- Weibull probability plot (graphical validation)  
- Kolmogorov–Smirnov test  
- Anderson–Darling test  

 These confirm that the Weibull model adequately represents the data.

---

## Key Findings

- Failure risk changes over time depending on Weibull parameters   
- Weibull distribution provides flexible modeling of reliability behavior  
- Survival analysis enables meaningful interpretation of time-to-event data  

---

## Skills Demonstrated

- Survival analysis  
- Parametric modeling (Weibull distribution)  
- Time-to-event data simulation  
- Handling censored data  
- Reliability analysis (MTTF, B-life)  
- Statistical validation and goodness-of-fit testing  
- Translating statistical models into practical insights  
