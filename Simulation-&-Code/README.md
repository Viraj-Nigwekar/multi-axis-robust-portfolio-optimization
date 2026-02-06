# Multi-Axis Robust Portfolio Optimization  
**Simulation and Empirical Analysis Repository**

This repository contains the primary simulation notebook used in the empirical analysis of the research paper **_Multi-Axis Robust Portfolio Optimization_**.
The notebook implements a unified robustness framework for mean–variance portfolio optimization and serves as the end-to-end computational pipeline for all portfolio simulations, covariance estimation procedures, and robustness diagnostics reported in the paper.

---

## Overview

The implemented framework addresses multiple sources of estimation uncertainty in portfolio construction through a unified, practitioner-oriented design.

Key components include:

- **Shrinkage Covariance Estimation**  
  Ledoit–Wolf–style regularization to stabilize noisy sample covariance matrices.

- **Bootstrap Aggregation**  
  Resampled covariance estimation with aggregation to reduce sampling variability and estimation risk.

- **Parametric Modeling (Geometric Brownian Motion)**  
  Forward-looking covariance generation using GBM-based stress simulations.

- **Unified Multi-Axis Ensemble**  
  Integration of structural, sampling, and parametric covariance estimates into a single ensemble estimator.

- **Markowitz Optimization**  
  Efficient frontier construction and risk–return analysis under multiple robustness regimes.

- **Out-of-Sample Evaluation**  
  Rolling-window backtesting using raw Close prices to ensure consistency and avoid data-adjustment artifacts.

- **Figures and Diagnostics**  
  All plots and diagnostic outputs used for empirical interpretation and robustness assessment.

---

## Purpose

This repository is intended to:

- Enable **full reproducibility** of the empirical results.
- Provide a transparent reference implementation of multi-axis robustness techniques.
- Support practitioner and research exploration of robust portfolio construction.
- Generate the figures and diagnostics used in the submitted manuscript.

---

## Data and Reproducibility

- Market data is **not included** in this repository.  
  The notebook specifies a fixed ticker universe and automatically downloads corresponding raw Close price data when executed.

- All simulations are fully scripted and reproducible conditional on random seeds.

---

## Use of AI Assistance

All model design, mathematical formulation, and core implementation logic were developed by the author.

AI-based tools were used **solely as auxiliary assistance** for:
- code formatting and organization,
- improving readability and comments,
- debugging and error tracing,
- and documentation and markdown polishing.

AI systems were **not used** to generate research ideas, modeling decisions, or empirical conclusions.

---

## Notes

- Results correspond to the empirical analysis underlying the submitted manuscript and may evolve if additional robustness checks or refinements are incorporated.
- This code is provided for **research and educational purposes** and is not intended as production trading infrastructure.
- ⚠️ Note: All reported Sharpe ratios are computed using daily out-of-sample returns under a rolling estimation framework. Equal-weight and GMV portfolios are included as baseline sanity checks.

