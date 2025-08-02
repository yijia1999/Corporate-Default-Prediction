# Corporate Default Risk Analysis
This repository contains two main Python Jupyter Notebooks focused on analyzing and predicting corporate default risk using structural credit risk models and machine learning techniques. The work is based on data from CRSP, COMPUSTAT, and macroeconomic indicators, developed as part of advanced coursework in Quantitative and Computational Finance.

## `notebook1.ipynb`: Distance to Default (DD) and Probability of Default (PD) Estimation
Implements three methods for computing Distance to Default and Probability of Default using the KMV model framework:

### Method 1: Naive KMV Estimation

A simplified approximation using market equity, debt, and stock volatility.

Fast to compute, useful for benchmarking.

### Method 2: Direct Estimation (Black-Scholes Approach)

Solves a system of nonlinear equations derived from the Merton model using observed equity volatility.

Provides more accurate firm value and asset volatility estimates.

### Method 3: Iterative KMV Estimation

Starts with an initial guess and iteratively refines estimates of firm value and asset volatility.

More time-consuming but closely follows the industry-standard KMV method.

All three approaches are applied to firm-level financial data across multiple years. The results include summary statistics, distribution plots, and macroeconomic overlays (e.g., recession indicators, BAA spread, financial stress index).

## `notebook2.ipynb`: Corporate Default Prediction using Machine Learning and Hazard Models
Builds predictive models to estimate the probability of corporate bankruptcy using financial covariates motivated by economic theory (e.g., leverage, profitability, liquidity, firm size). The process includes:

Feature Engineering: Selection and computation of variables based on economic rationale and prior literature.

Model Evaluation: In-sample (1964–1990) and out-of-sample (1991–2019) performance assessment.
