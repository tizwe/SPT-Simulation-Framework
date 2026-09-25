# SPT Simulation Framework

A Python framework for simulating markets and functionally generated portfolios in Stochastic Portfolio Theory (SPT).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tizwe/SPT-Simulation-Framework/blob/main/SPT_Simulation_Framework.ipynb)

The notebook runs directly in the browser via Google Colab, no installation needed.

## Features

- **Markets:** simulate stock prices driven by several Brownian motions, with random or custom covariance matrices, a common market factor and optional rank-based drifts.
- **Portfolios:** market, equally weighted, constant-weight and buy-and-hold portfolios, or any custom update rule, with adjustable rebalancing frequency.
- **Functionally generated portfolios:** define a generating function G, and the portfolio weights are computed automatically via automatic differentiation.
- **Growth-optimal portfolio:** solved as a quadratic program, including a study of estimation errors in the expected returns.
- **Relative arbitrage:** Monte Carlo estimation of the arbitrage horizon for the quadratic generating function.
- **Interactive visualizations** to explore how parameters such as volatility or the market factor affect the results.

## Running locally

Uncomment the local installation line at the top of the notebook, or run

    pip install numpy pandas scipy matplotlib plotly ipywidgets tqdm joblib torch cvxpy nbformat

## Background

Developed as part of my MSc thesis *Relative Arbitrage in Diverse Markets: Developing a Framework for Functionally Generated Portfolios* at the University of Konstanz (2026).

The parameters in the notebook are reduced so that it runs quickly in Colab. The values used for the figures in the thesis are noted in the code comments.

## License

MIT
