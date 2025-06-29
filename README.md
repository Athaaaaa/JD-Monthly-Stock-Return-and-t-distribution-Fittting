# JD-Monthly-Stock-Return-and-t-distribution-Fittting

# JD Monthly Stock Return Analysis and t-Distribution Fitting

This project involves financial econometrics analysis of **JD.com (京东)** stock. It focuses on computing **monthly logarithmic returns** based on adjusted closing prices, and fitting the **generalized t-distribution** to the return data using **Maximum Likelihood Estimation (MLE)** and comparing it with **fitdistrplus** package results.

## Files Included

* `JD.csv`: Raw stock price data (adjusted monthly close)
* `jd_return_analysis.R`: R script for calculating returns and fitting distributions
* `Report.pdf`: Analysis report 

## Features

* Calculates **logarithmic monthly returns** using R
* Implements **custom t-distribution fitting** via `optim()` function (no external packages)
* Compares results with the standard `fitdistrplus` package
* Visual and textual analysis included in the report

## Methodology

1. **Monthly Log Returns**:


2. **Custom Generalized t-distribution PDF**:



3. **MLE Estimation**:


4. **fitdistrplus Comparison**:


## Results

| Method       | Location  | Scale    | Shape (df) |
| ------------ | --------- | -------- | ---------- |
| MLE (manual) | -0.001561 | 0.025492 | 6.711      |
| fitdistrplus | -0.001564 | 0.025456 | 6.709      |

Both methods produce highly consistent results, supporting the robustness and reliability of the parameter estimation.

## Conclusion

The project validates the **generalized t-distribution** as a suitable model for JD.com's return data due to its flexibility in handling outliers and fat tails. The close match between manual MLE and `fitdistrplus` fitting confirms consistency and methodological soundness.

