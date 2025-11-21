\begin{verbatim}
# Multi-Axis Robust Portfolio Optimization

This repository contains the code, simulations, and empirical pipeline for a unified multi-axis robustness framework in portfolio optimization.  
The methodology combines shrinkage estimation, bootstrap aggregation, and parametric modeling (GBM-based) to improve stability and out-of-sample performance in mean–variance portfolios.

The notebook included here was used to generate the experimental results for my accompanying research paper (currently under preparation).

---

## Overview

Traditional Markowitz optimization is highly sensitive to noise in sample means and covariances.  
This project implements a multi-axis robustness ensemble designed to mitigate estimation error by integrating:

- **Axis 1 — Shrinkage Estimation**  
  Regularization of covariance matrices using shrinkage techniques.

- **Axis 2 — Bootstrap Aggregation**  
  Covariance resampling, variance reduction, and robust averaging.

- **Axis 3 — Parametric Modeling**  
  GBM-based covariance estimation to incorporate forward-looking distributional structure.

Each axis produces an independent covariance estimate.  
The final portfolio is constructed using a unified ensemble of these estimates.

---

## Repository Structure

multi-axis-robust-portfolio-optimization/
│
├── notebooks/
│   └── robustness.ipynb        # Main research notebook
│
├── figures/                    # Saved charts and plots
│   ├── ...
│
├── requirements.txt            # Python dependencies
│
└── README.md                   # Project documentation

---

## Usage

1. Clone the repository:
   git clone https://github.com/<your-username>/multi-axis-robust-portfolio-optimization

2. Install dependencies:
   pip install -r requirements.txt

3. Open the main notebook:
   notebooks/robustness.ipynb

---

## Data

All experiments use **raw Close prices** from Yahoo Finance.  
Data is not included in this repository.  
Users may download identical series using the ticker list in the notebook.

---

## Status

- Research notebook: Complete  
- Paper: In preparation (theoretical sections under revision)  
- Results: Being finalized for publication-level presentation  

---

## License

This repository is currently private and does not include a license.  
A license will be added upon public release.
\end{verbatim}
