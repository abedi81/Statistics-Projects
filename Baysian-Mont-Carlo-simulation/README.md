# Bayesian Inference via Monte Carlo Simulation

## Overview

This project demonstrates Bayesian inference using Monte Carlo simulation in the context of a medical testing problem.

The goal is to estimate the probability that an individual has a disease given a positive test result, and to show how simulation can approximate the true posterior probability.

Instead of relying only on analytical formulas, the project uses repeated random sampling to build intuition about how Bayesian updating works in practice.

---

## Problem Setup

The simulation models a realistic scenario:

- A rare disease with low prevalence (prior probability)  
- A medical test with:
  - High true positive rate (sensitivity)  
  - Non-negligible false positive rate  

The key question is:

 *Given a positive test result, what is the probability that the individual actually has the disease?*

---

## Methodology

The project follows a simulation-based Bayesian approach:

1. Generate a population based on a prior probability of disease  
2. Simulate test outcomes using:
   - True positive rate (TPR)  
   - False positive rate (FPR)  
3. Count:
   - True positives  
   - False positives  
4. Estimate the posterior probability using simulated data  

This process is repeated multiple times to understand variability and convergence.

---

## Monte Carlo Simulation

Multiple simulations are run under varying conditions:

- Different prior probabilities  
- Different test accuracies (TPR, FPR)  
- Increasing number of iterations  

 This allows us to observe how the estimated posterior evolves across repeated experiments. 

---

## Analytical Benchmark

The simulation results are compared to the analytical Bayesian solution.

 This provides a reference point to evaluate how accurately the simulation approximates the true posterior.

---

## Key Findings

- The posterior probability is much lower than expected due to false positives  
- Even accurate tests can produce misleading results when the disease is rare  
- Monte Carlo simulation converges to the analytical solution as the number of iterations increases  
- The distribution of posterior estimates becomes more stable with larger sample sizes  

---

## Convergence Behavior

- With small iterations there is high variability  
- With larger iterations we see stable mean and tighter distribution  
- The simulated mean approaches the analytical posterior  

 This demonstrates the Law of Large Numbers in a Bayesian setting  

---

## Visualization

The project includes:

- Histograms of posterior probabilities  
- Comparison between simulated and analytical values  
- Fitted probability distributions  

These visualizations help illustrate how uncertainty decreases as simulation size increases.

---

## Key Insights

- Bayesian reasoning depends heavily on prior probabilities  
- False positives can dominate outcomes in rare-event settings  
- Simulation provides an intuitive way to understand Bayesian updates  
- Increasing sample size improves estimate reliability  

---

## Skills Demonstrated

- Bayesian inference  
- Monte Carlo simulation  
- Probabilistic modeling  
- Statistical convergence analysis  
- Distribution fitting and visualization  
- Translating theory into simulation-based intuition  
