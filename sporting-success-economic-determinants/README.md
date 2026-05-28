# What Drives International Sporting Success?

## Overview
Why do some countries consistently dominate global sport while others struggle to make a name for themselves? This project investigates how economic strength relates to international sporting success. Bernard and Busse (2004) showed that GDP per capita, population and hosting are strong predictors of Olympic success. Building on their findings, this analysis extends to the seven most recent Summer Olympic Games (2000–2024) and examines whether similar effects are found in international football using FIFA World Rankings. A Poisson model is then used to predict medal counts for the Paris 2024 Olympics.

This was submitted as coursework for the Econometrics with Python module (ECONM0014) at the University of Bristol, achieving a mark of 78%.

## Key Findings
- Economic strength is a significant predictor of both Olympic medal counts
and FIFA World Rankings, after controlling for population
- Hosting the Olympics provides a meaningful boost to medal performance
- In football, confederation membership matters — Europe and South America
consistently outperform other regions
- The Poisson model achieves a mean absolute error of 3.63 medals for Paris
2024, an improvement on the 4.3 reported by Bernard and Busse (2004) for
Sydney 2000
- Some countries match predictions almost perfectly (France as hosts, Sweden,
Kazakhstan), while Australia and Great Britain substantially outperform
their predicted totals
- Notable outliers include India, whose Olympic performance remains limited
despite its population size, and Saudi Arabia, predicted to win almost 20
medals due to high GDP per capita but winning none
- Causal conclusions cannot be drawn due to likely endogeneity from omitted
variables such as sports investment, cultural priorities and domestic league
strength

## Methodology
- OLS regression of Olympic medal counts and FIFA World Rankings on GDP 
per capita, population, hosting status and confederation membership
- Poisson regression for medal count prediction, exploiting the non-negative
integer nature of the dependent variable
- Out-of-sample prediction for Paris 2024 with evaluation against actual
results
- Implemented in Python

## Files
- `sporting-success-economic-determinants.zip` — includes Python script, 
final dataset and images

## Tools
Python
