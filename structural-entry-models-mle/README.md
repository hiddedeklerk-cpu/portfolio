# Structural Entry Models — MLE and Simulation

## Overview
This project estimates structural entry models following Bresnahan and 
Reiss (1991) and Berry (1992), using data on tyre dealers across US towns. 
A binary probit entry model is estimated by Maximum Likelihood, with the 
log-likelihood, gradient and Hessian derived analytically and implemented 
from scratch in MATLAB. Results are cross-validated against Stata. The 
project then extends to a Berry (1992) simulation framework incorporating 
firm heterogeneity to estimate the expected number of market entrants.

This was submitted as coursework for the Empirical Industrial Organisation 
module (ECONM0013) at the University of Bristol, achieving a mark of 100%.

## Key Findings
- MLE estimates are almost identical across MATLAB and Stata implementations,
validating the analytical gradient and Hessian derivations
- The majority of structural parameters are statistically insignificant,
consistent with Bresnahan and Reiss (1991), likely reflecting a homogeneous
sample after restricting to monopolistic markets
- The simulation reveals a systematic over-prediction of entrants,
particularly in markets with fewer observed entrants, consistent with
Berry (1992)'s finding that ignoring firm heterogeneity leads to upward
bias
- Results highlight the trade-off between the simplicity of symmetric 
entry models and the realism of firm heterogeneity approaches

## Methodology
- Analytical derivation of the log-likelihood, gradient and Hessian for 
a nonlinear binary probit model
- Maximum likelihood estimation using MATLAB's fminunc with trust-region 
algorithm, supplying analytical derivatives
- Cross-validation of MATLAB estimates against Stata ml command
- Berry (1992) simulation with 1,000 draws per market to estimate expected 
number of entrants under firm heterogeneity
- Discussion of Toivanen and Waterson (2005) on learning effects in a 
fast food duopoly

## Files
- `structural_entry_models.pdf` — full write-up including derivations, 
results, simulation and all code

## Tools
MATLAB, Stata
