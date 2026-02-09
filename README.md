# Multi-Axis Robust Portfolio Optimization

This repository contains the empirical pipeline and implementation for a **unified multi-axis robustness framework** in mean–variance portfolio optimization.  
The framework integrates shrinkage-based covariance regularization, bootstrap aggregation, and parametric (GBM-based) modeling to improve **stability, robustness, and out-of-sample behavior** under estimation uncertainty.

The code in this repository was used to generate the experimental results reported in the accompanying research paper.

---

## Key Idea

Classical Markowitz portfolio optimization is highly sensitive to noise in estimated means and covariances.  
Rather than addressing estimation error along a single dimension, this project treats robustness as an **ensemble property** arising from diversification across multiple uncertainty axes.

The framework combines:

- **Structural robustness** via covariance shrinkage  
- **Sampling robustness** via bootstrap aggregation  
- **Parametric robustness** via scenario-based (GBM) modeling  

Each axis produces an independent portfolio allocation.  
The final portfolio is constructed as an equal-weight ensemble of these allocations to reduce variance without introducing additional tuning parameters.

---

## Usage

1. Clone the repository:
{```bash
git clone https://github.com/Viraj-Nigwekar/multi-axis-robust-portfolio-optimization.git}
cd multi-axis-robust-portfolio-optimization

# Multi-Axis Robust Portfolio Optimization

This repository contains the empirical pipeline and implementation for a **unified multi-axis robustness framework** in mean–variance portfolio optimization.  
The framework integrates shrinkage-based covariance regularization, bootstrap aggregation, and parametric (GBM-based) modeling to improve **stability, robustness, and out-of-sample behavior** under estimation uncertainty.

The code in this repository was used to generate the experimental results reported in the accompanying research paper.

---

## Key Idea

Classical Markowitz portfolio optimization is highly sensitive to noise in estimated means and covariances.  
Rather than addressing estimation error along a single dimension, this project treats robustness as an **ensemble property** arising from diversification across multiple uncertainty axes.

The framework combines:

- **Structural robustness** via covariance shrinkage  
- **Sampling robustness** via bootstrap aggregation  
- **Parametric robustness** via scenario-based (GBM) modeling  

Each axis produces an independent portfolio allocation.  
The final portfolio is constructed as an equal-weight ensemble of these allocations to reduce variance without introducing additional tuning parameters.

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/Viraj-Nigwekar/multi-axis-robust-portfolio-optimization.git
cd multi-axis-robust-portfolio-optimization
# Multi-Axis Robust Portfolio Optimization

This repository contains the empirical pipeline and implementation for a **unified multi-axis robustness framework** in mean–variance portfolio optimization.  
The framework integrates shrinkage-based covariance regularization, bootstrap aggregation, and parametric (GBM-based) modeling to improve **stability, robustness, and out-of-sample behavior** under estimation uncertainty.

The code in this repository was used to generate the experimental results reported in the accompanying research paper.

---

## Key Idea

Classical Markowitz portfolio optimization is highly sensitive to noise in estimated means and covariances.  
Rather than addressing estimation error along a single dimension, this project treats robustness as an **ensemble property** arising from diversification across multiple uncertainty axes.

The framework combines:

- **Structural robustness** via covariance shrinkage  
- **Sampling robustness** via bootstrap aggregation  
- **Parametric robustness** via scenario-based (GBM) modeling  

Each axis produces an independent portfolio allocation.  
The final portfolio is constructed as an equal-weight ensemble of these allocations to reduce variance without introducing additional tuning parameters.

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/Viraj-Nigwekar/multi-axis-robust-portfolio-optimization.git
cd multi-axis-robust-portfolio-optimization

2. Install dependencies:
pip install -r requirements.txt

3. Run the analysis:
jupyter notebook notebooks/robustness.ipynb

The notebook executes the full rolling-window experiment, including portfolio construction, evaluation, and diagnostic analysis.

Data

All experiments use daily raw Close prices sourced from Stooq.
Price data is not included in this repository.

The notebook contains the complete ticker list and data-loading logic required to reproduce the results.

Reproducibility

Fixed hyperparameters are used across all methods

All portfolios are evaluated using rolling out-of-sample windows

Sharpe ratios are computed from daily out-of-sample returns and annualized consistently

Saved figures correspond directly to notebook outputs

Status

Research notebook: Complete

Empirical results: Complete

Paper: Complete

License

This repository is currently public and does not include a license.
All code is provided for research and educational purposes.

Notes

This repository accompanies a research paper and emphasizes methodological clarity, reproducibility, and stability, rather than production deployment.
