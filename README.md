# Bayesian Parameter Estimation of Cosmological Models using MCMC

## Overview

I estimate two cosmological parameters — the Hubble constant (H₀) and the matter density parameter (Ωm) — from observational data on galaxy expansion rates. I built the Metropolis-Hastings sampler from scratch rather than calling a library, mostly because I wanted to understand what's actually happening at each step.

## Workflow

- Define the cosmological model H(z; H₀, Ωm)
- Build the Gaussian likelihood and prior distributions
- Implement the Metropolis-Hastings proposal and acceptance step
- Run the chain (1M steps, 100k burn-in)
- Check convergence and visualize the posterior distributions

## Results

With a uniform prior, the 68% confidence intervals land at H₀ ∈ (67.2, 70.8) km/s/Mpc and Ωm ∈ (0.308, 0.322). Switching to an informative Gaussian prior on Ωm tightens both intervals — expected, since you're feeding the sampler more information. Acceptance rate sits around 9.5%, slightly below the ~23% optimum for a 2-parameter sampler, which suggests the proposal widths could be tuned tighter.

## Dataset

[Download here](https://drive.google.com/file/d/1Z9YyuZSNVbWEV0S2HT1GRVama11JNr8R/view?usp=drive_link)
