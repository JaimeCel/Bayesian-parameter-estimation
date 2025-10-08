# Bayesian Parameter Estimation of Cosmological Models using MCMC
## Overview
In this project, we estimate two fundamental parameters in cosmology: the Hubble constant and the matter density parameter.
We employ a Bayesian framework, specifically using the Markov Chain Monte Carlo (MCMC) method, to infer their most probable values based on observational data.
The notebook walks through defining a model, constructing posterior and proposal functions, and running an MCMC chain to estimate parameters. 

---

##  Workflow 
- Define the cosmological model.
- Construct the posterior probability function combining priors and likelihood.
- Implement the proposal function for parameter updates.
- Run the MCMC chain.
- Analyze convergence and burn in regions and visualize parameter estimations.
---

##  Results
The notebook generates MCMC trace and posterior distribution plots, yielding values for the Hubble constant and matter density parameter.
This enables us to determine the 68% confidence intervals for each estimated parameter.

---

##  Notes
The dataset is stored in a Google Drive folder for size issues. You can download it from this link [Dataset](https://drive.google.com/file/d/1Z9YyuZSNVbWEV0S2HT1GRVama11JNr8R/view?usp=drive_link)
