# Robustness Notebook Overview

This notebook implements the full unified multi-axis robustness framework used in the empirical analysis of the research project *Multi-Axis Robust Portfolio Optimization*. It serves as the computational backbone for generating simulations, covariance estimates, and portfolio results.

## Contents

The notebook includes:

- **Shrinkage Covariance Estimation**  
  Ledoit–Wolf style regularization for stabilizing covariance matrices.

- **Bootstrap Aggregation**  
  Resampled covariance estimates with variance reduction and robust averaging.

- **Parametric Modeling (GBM)**  
  Forward-looking covariance generation using Geometric Brownian Motion.

- **Unified Ensemble Construction**  
  Combination of shrinkage, bootstrap, and parametric covariance estimates.

- **Efficient Frontier & Risk Analysis**  
  Markowitz optimization under multiple robustness regimes.

- **Out-of-Sample Evaluation**  
  Rolling-window simulations using raw Close prices.

- **Figure Generation**  
  All plots and heatmaps used for empirical interpretation.

## Purpose

This notebook is designed for:

- Reproducible research
- Empirical validation of robustness methods
- Generation of figures for the accompanying paper
- Transparent documentation of the simulation pipeline

## Notes

- Data is not included.  
  Use the ticker list inside the notebook to download identical raw Close prices.

- All results are preliminary and may be updated as the theoretical sections of the paper are refined.

