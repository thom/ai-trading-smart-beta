# Udacity Artificial Intelligence for Trading Nanodegree - Project: Smart Beta and Portfolio Optimization

- [Introduction](#introduction)
- [Overview](#overview)
- [Getting started](#getting-started)
- [Dependencies](#dependencies)
- [Instructions](#instructions)
- [References](#references)
- [License](#license)

## Introduction

This project builds a smart beta portfolio and compares it to a benchmark index. The portfolio is built using quadratic programming to optimize the weights. The code rebalances the portfolio and calculates turn over to evaluate the performance. This metric is used to find the optimal rebalancing frequency. To find out how well the smart beta portfolio did, the project calculates the tracking error against the index.

## Overview

Smart beta has a broad meaning, but we can say in practice that when we use the universe of stocks from an index, and then apply some weighting scheme other than market cap weighting, it can be considered a type of smart beta fund. A Smart Beta portfolio generally gives investors exposure or "beta" to one or more types of market characteristics (or factors) that are believed to predict prices while giving investors a diversified broad exposure to a particular market. Smart Beta portfolios generally target momentum, earnings quality, low volatility, and dividends or some combination. Smart Beta Portfolios are generally rebalanced infrequently and follow relatively simple rules or algorithms that are passively managed. Model changes to these types of funds are also rare requiring prospectus filings with US Security and Exchange Commission in the case of US focused mutual funds or ETFs. Smart Beta portfolios are generally long-only, they do not short stocks.

In contrast, a purely alpha-focused quantitative fund may use multiple models or algorithms to create a portfolio. The portfolio manager retains discretion in upgrading or changing the types of models and how often to rebalance the portfolio in attempt to maximize performance in comparison to a stock benchmark. Managers may have discretion to short stocks in portfolios.

Imagine you're a portfolio manager, and wish to try out some different portfolio weighting methods.

One way to design portfolio is to look at certain accounting measures (fundamentals) that, based on past trends, indicate stocks that produce better results.

For instance, you may start with a hypothesis that dividend-issuing stocks tend to perform better than stocks that do not. This may not always be true of all companies; for instance, Apple does not issue dividends, but has had good historical performance. The hypothesis about dividend-paying stocks may go something like this:

Companies that regularly issue dividends may also be more prudent in allocating their available cash, and may indicate that they are more conscious of prioritizing shareholder interests. For example, a CEO may decide to reinvest cash into pet projects that produce low returns. Or, the CEO may do some analysis, identify that reinvesting within the company produces lower returns compared to a diversified portfolio, and so decide that shareholders would be better served if they were given the cash (in the form of dividends). So according to this hypothesis, dividends may be both a proxy for how the company is doing (in terms of earnings and cash flow), but also a signal that the company acts in the best interest of its shareholders. Of course, it's important to test whether this works in practice.

You may also have another hypothesis, with which you wish to design a portfolio that can then be made into an ETF. You may find that investors may wish to invest in passive beta funds, but wish to have less risk exposure (less volatility) in their investments. The goal of having a low volatility fund that still produces returns similar to an index may be appealing to investors who have a shorter investment time horizon, and so are more risk averse.

So the objective of your proposed portfolio is to design a portfolio that closely tracks an index, while also minimizing the portfolio variance. Also, if this portfolio can match the returns of the index with less volatility, then it has a higher risk-adjusted return (same return, lower volatility).

Smart Beta ETFs can be designed with both of these two general methods (among others): alternative weighting and minimum volatility ETF.

## Getting started

1. Fork this repository
2. Ensure you have all the dependencies
3. Follow the instructions below

## Dependencies

Install one of the following Python virtual environment managers:

- [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html), or
- [Virtualenv](https://virtualenv.pypa.io/), or
- [Pipenv](https://pipenv.pypa.io/)

The following instructions refer to Miniconda. Check out the respective links above in case you need help with any of the other methods.

## Instructions

Create a new `ai-trading-smart-beta` Conda environment installing the required packages:

```bash
conda create --file ai-trading-smart-beta.yml
```

Activate the environment:

```bash
conda activate ai-trading-smart-beta
```

Start Jupyter:

```bash
jupyter notebook
```

Open the `smart_beta_and_portfolio_optimization.ipynb` notebook and follow the instructions.

## References

TBD

- [Pipenv vs virtualenv vs conda environment](https://medium.com/@krishnaregmi/pipenv-vs-virtualenv-vs-conda-environment-3dde3f6869ed)
- [Miniconda installation](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)
- [Conda cheatsheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)
- [Jupyter Notebook Cheat Sheet](https://www.edureka.co/blog/wp-content/uploads/2018/10/Jupyter_Notebook_CheatSheet_Edureka.pdf)
- [Jupyter Lab Cheat Sheet](https://www.anaconda.com/wp-content/uploads/2019/03/11-2018-JupyterLab-Notebook-Cheatsheet.pdf)

## License

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2021 © [Thomas Weibel](https://github.com/thom).
