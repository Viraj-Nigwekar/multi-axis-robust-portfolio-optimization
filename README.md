# Multi-Axis Robust Portfolio Optimization

A reproducible research implementation of a unified multi-axis robustness framework for mean–variance portfolio optimization.

This repository contains the complete empirical pipeline used to evaluate a portfolio optimization framework that integrates covariance shrinkage, bootstrap aggregation, and parametric scenario modeling. The implementation emphasizes reproducibility, methodological clarity, and robust out-of-sample evaluation under estimation uncertainty.

The accompanying research paper is available on SSRN:

**SSRN:** *https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5874942*

---

# Overview

Classical mean–variance (Markowitz) portfolio optimization is highly sensitive to estimation error in expected returns and covariance matrices. Small changes in these estimates can produce substantially different portfolio allocations.

Rather than addressing a single source of uncertainty, this project treats robustness as an ensemble property by combining multiple complementary robustness mechanisms into a unified portfolio construction framework.

The framework integrates three independent robustness axes:

* **Structural Robustness** — Covariance shrinkage regularization
* **Sampling Robustness** — Bootstrap aggregation
* **Parametric Robustness** — Geometric Brownian Motion (GBM) scenario modeling

Each robustness axis independently generates a portfolio allocation. The final portfolio is constructed as an equal-weight ensemble of these allocations, providing improved stability while avoiding additional tuning parameters.

---

# Features

* Multi-axis robust portfolio optimization framework
* Covariance shrinkage estimation
* Bootstrap portfolio aggregation
* GBM-based scenario generation
* Rolling-window out-of-sample evaluation
* Portfolio performance analysis
* Risk-adjusted performance metrics
* Fully reproducible research pipeline


---

# Installation

Clone the repository:

```bash
git clone https://github.com/Viraj-Nigwekar/multi-axis-robust-portfolio-optimization.git
cd multi-axis-robust-portfolio-optimization
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

# Usage

Launch the notebook:

```bash
jupyter notebook notebooks/robustness.ipynb
```

The notebook executes the complete experimental pipeline, including:

* Data loading
* Covariance estimation
* Portfolio construction
* Rolling-window evaluation
* Performance comparison
* Diagnostic analysis
* Figure generation

---

# Data

The experiments use daily historical closing prices obtained from **Stooq**.

To keep the repository lightweight, raw market data is not included. The notebook contains the complete ticker list together with the data-loading logic required to reproduce every experiment.

No proprietary datasets are required.

---

# Reproducibility

This repository is designed to facilitate reproducible research.

The implementation uses:

* Fixed hyperparameters across all methods
* Consistent rolling out-of-sample evaluation
* Standardized annualized performance metrics
* Reproducible figure generation
* Notebook outputs that correspond directly to the reported experimental results

---

# Outputs

Running the notebook generates:

* Portfolio allocation comparisons
* Rolling cumulative return curves
* Risk–return analysis
* Sharpe ratio comparisons
* Drawdown analysis
* Performance summary statistics
* Publication-quality figures

---

# Project Status

* ✅ Research implementation complete
* ✅ Experimental evaluation complete
* ✅ Manuscript complete
* 🔄 Ongoing maintenance and documentation improvements

---

# Citation

If you use this repository in your research, please cite the accompanying paper.

```bibtex
% Add your BibTeX citation here after publication or SSRN upload.
```

---

# License

This project is licensed under the MIT License. See the LICENSE file for details.

---

# Notes

This repository accompanies an academic research paper and is intended primarily as a reproducible research implementation rather than a production trading system.

Contributions, suggestions, and constructive feedback are welcome.
