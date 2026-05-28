# ECB Monetary Policy and Eurozone Financial Markets

## Overview
This project examines how ECB unconventional monetary policy — including 
negative interest rates and quantitative easing — affected Eurozone equity 
markets and exchange rates over 2015–2018. Using daily data on the Euro 
STOXX 50 index, the USD/EUR exchange rate and the 3-month EURIBOR rate, 
a trivariate Vector Error Correction Model (VECM) is estimated to capture 
both long-run and short-run dynamics between the three variables.

This was submitted as coursework for the Applied Financial Econometrics 
module (ECONM0009) at the University of Bristol, achieving a mark of 88%.

## Key Findings
- Cointegration is detected at the 1% significance level across all 
specifications, suggesting a long-run relationship between equity markets, 
exchange rates and interest rates
- A positive long-run relationship is found between the Euro/USD exchange 
rate and the Euro STOXX 50, consistent with the capital flows channel
- The positive long-run relationship between EURIBOR and equity prices 
challenges standard monetary theory, potentially reflecting improved 
investor confidence during the unconventional policy period
- In the short run, equity markets appear to lead exchange rates, confirmed 
by impulse response functions
- Diagnostic checks suggest possible fractional cointegration (d = 0.873 
via Robinson (1995)), challenging the strict I(1) assumption

## Methodology
- Augmented Dickey-Fuller unit root tests with Schwert (1989) lag selection
- Johansen (1991) trace test for cointegration across three specifications
- VECM estimation with analytical error correction terms
- Bootstrap impulse response functions over a 20-day horizon
- Robinson (1995) semiparametric long memory test on cointegrating residuals
- Diagnostic checks: serial correlation, normality, ARCH effects

## Files
- `ecb_monetary_policy_vecm.pdf` — full write-up including methodology, 
results, discussion and all code

## Tools
R (xts, urca, vars), STATA
