# Error vs Residual in Regression: A Simulation-Based Analysis

## Overview

This project demonstrates the fundamental difference between **true errors** and **residuals** in regression analysis using simulation.

The goal is to show how Ordinary Least Squares (OLS) behaves in practice and to clarify key theoretical concepts such as unbiasedness, orthogonality conditions, and the role of randomness in estimation.

---

## Motivation

In regression analysis, the terms *error* and *residual* are often confused.

- **Error (uᵢ):** Unobserved, true random noise in the population  
- **Residual (ûᵢ):** Estimated error from the sample model  

This project uses simulation to show that these two are fundamentally different, even though they are often treated similarly in theory.

---

## Methodology

The project follows a simulation-based approach:

1. Generate independent variable (x) from a uniform distribution  
2. Generate true error (u) from a normal distribution  
3. Construct outcome using the true model:

   y = β₀ + β₁x + u  

4. Estimate the model using OLS  
5. Compare:
   - True errors (uᵢ)  
   - Estimated residuals (ûᵢ)  

6. Repeat simulations to observe variability and convergence :contentReference[oaicite:0]{index=0}

---

## Key Concepts Demonstrated

### 1. OLS Unbiasedness

- Estimated coefficients are close to true values  
- Across many samples, estimates converge to true parameters  

 This confirms that OLS is unbiased

---

### 2. Residual Properties (Always True in Sample)

OLS residuals satisfy:

- Sum of residuals = 0  
- Sum of xᵢ × residuals = 0  

 These are **mechanical properties** of OLS optimization  

---

### 3. True Error Behavior (Not Forced)

True errors:

- Do NOT sum to zero in a given sample  
- Are NOT guaranteed to be uncorrelated with x in finite samples  

 These properties hold only **in expectation**, not in every sample  

---

## Key Findings

- Residuals are constructed to satisfy OLS conditions exactly  
- True errors are random and do not satisfy these conditions in finite samples  
- OLS estimates vary across samples due to randomness  
- As sample size increases, estimates and averages converge to true values  

---

## Statistical Insight

This project highlights an important distinction:

 OLS assumptions apply to **true errors (population level)**  
 OLS properties apply to **residuals (sample level)**  

Confusing these two can lead to misunderstanding regression results.

---

## Convergence Behavior

- Small samples → more variation in estimates  
- Larger samples → estimates closer to true values  
- Demonstrates the **Law of Large Numbers**

---

## Why This Matters

Understanding the difference between errors and residuals is critical for:

- Correct interpretation of regression models  
- Avoiding misconceptions about OLS assumptions  
- Understanding sampling variability  
- Applying econometric methods correctly  

---

## Skills Demonstrated

- Simulation-based statistical analysis  
- Regression modeling (OLS)  
- Econometric reasoning  
- Understanding of bias and consistency  
- Law of Large Numbers in practice  
- Translating theory into empirical intuition  
