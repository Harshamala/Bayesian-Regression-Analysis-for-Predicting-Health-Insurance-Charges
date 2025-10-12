# Bayesian-Regression-Analysis-for-Predicting-Health-Insurance-Charges
This study employs Bayesian regression to model health insurance charges, incorporating variables such as age, gender, BMI, and smoking status

This project applies **Bayesian regression modeling** to predict individual health insurance charges based on demographic and lifestyle variables such as **age**, **gender**, **BMI**, and **smoking status**.  
The goal is to understand how these factors contribute to variations in insurance costs and quantify the uncertainty around parameter estimates using Bayesian methods.

------------

## Overview

Two Bayesian regression models were compared:

### **Model 1: Raw Charges as Response**
- The dependent variable (`charges`) is used in its original scale.
- Captures the actual scale of the data but requires **robust priors and likelihoods** to handle heavy-tailed distributions.
- Useful for interpreting results in real monetary units.

### **Model 2: Log-Transformed Charges as Response**
- The natural logarithm of `charges` was modelled.
- The transformation reduces right skewness and stabilizes variance.
- Produces a more normally distributed response, leading to better model fit and convergence.

---

## Key Findings

- **Strong predictors:**  
  - `age`, `BMI`, and `smoking_status` significantly influence insurance charges.  
- **Weaker predictors:**  
  - `gender` and `number_of_children` show weaker or uncertain effects.
- **Model comparison:**  
  - The Gaussian likelihood provided **more stable estimates** and **credible intervals**.  
  - Bayesian R² values suggest the model explains a substantial portion of the variation in charges.
- **Diagnostics:**  
  - Convergence checks (`R̂ < 1.01`) indicate reliable posterior estimates.

---

## Practical Implications

- **Policy insight:** Smoking and high BMI drive higher insurance costs.  
- **Business impact:** Insurers can design fairer pricing strategies and incentivize healthier behavior.  
- **Methodological strength:** Bayesian modeling captures uncertainty and provides richer insights than traditional regression.

---

## Methodology

- Bayesian Linear Regression
- Posterior inference via MCMC sampling 
- Comparison via posterior summaries, credible intervals, and Bayesian R²
- Convergence checks: R̂

---

