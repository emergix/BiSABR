# BiSABR: A Bi-Dimensional SABR Framework for Spread Option Pricing

## 🧠 Overview

This repository introduces a powerful extension of the classical SABR model to a **bi-dimensional stochastic volatility framework**, tailored to accurately price **spread options**. By accounting for both asset-specific volatilities and cross-correlations—including stochastic co-movements—this model provides **a closed-form approximation** of the spread option price, along with a practical calibration strategy.

Presentation : [pres_SABR_BiSABR](./pdf/pres_SABR_BiSABR.pdf)

Demonstration : [pres_SABR_BiSABR](./pdf/Demonstration.pdf)

## 📈 Key Features

- ✅ **Closed-form formula** for implied normal volatility in spread options.
- ✅ **Handles transverse correlations** (e.g., between volatilities and underlying cross-assets).
- ✅ **Efficient calibration** using market data from vanilla and spread options.
- ✅ **Monte Carlo benchmark validation** confirms pricing precision.
- ✅ Implemented using symbolic computation and can be ported to C++ or Python.

## 📊 Why It Matters for Traders

Spread options are commonly used in:

- Commodities (e.g. WTI–Brent spreads),
- Energy (e.g. spark and crack spreads),
- Equities (e.g. dispersion and correlation trades),
- Fixed income (e.g. curve trades).

Yet, standard models like Black-Scholes or univariate SABR fail to accurately capture the **smile**, **skew**, and **vol of vol** seen in the spread option market.

**This model allows traders and quants to:**
- Capture **non-linear risks and convexity** in spread structures.
- Calibrate **hidden correlation structures** not visible in vanilla options.
- Perform **accurate pricing and hedging** without heavy simulation.

## 🧪 Components

| File | Description |
|------|-------------|
| `bisabr_spread_option.tex` | Main LaTeX source presenting the model and empirical results. |
| `BiSABR_Demonstration.nb` | Mathematica notebook for symbolic derivation of the formula. |
| `BISABR_Example.pdf` | Demonstrates pricing using the analytical formula. |
| `BiSABR_MonteCarlo.pdf` | Monte Carlo simulation validating the model. |
| `spreadoption_sabr2.pdf` | Application to market data and calibration of cross-correlations. |

## 🔧 How to Use

1. **Derive** the closed-form formula symbolically or reuse provided code.
2. **Calibrate** your SABR parameters for each asset from vanilla options.
3. **Fit** the transverse correlations using market quotes of spread options.
4. **Price** and **hedge** using the closed-form approximation (or benchmark with MC).

## 📚 Citation

If you use this model in research or production, please cite as:

