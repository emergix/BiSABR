# Mathematica Directory – BiSABR Spread Option Pricing

This directory contains the **symbolic derivations**, **demonstrations**, and **validation notebooks** used to develop and verify the closed-form BiSABR pricing model for spread options.

## 📂 Contents

| File | Description |
|------|-------------|
| `BiSABR_Demonstration.nb` | Main derivation notebook showing how the variance of the spread is computed symbolically. Includes Jacobian and covariance propagation. |
| `BISABR_Example.pdf` | Output from Mathematica showing how the analytical formula behaves under various parameter settings. |
| `BiSABR_MonteCarlo.pdf` | Monte Carlo simulations comparing analytical pricing with stochastic simulation. Includes antithetic variance reduction. |
| `spreadoption_sabr2.pdf` | Application of the formula to real-market spread options. Calibration of cross-asset and cross-volatility correlations. |

## 🧠 What This Directory Provides

- A **symbolic derivation environment** to manipulate SABR dynamics with full generality.
- Analytical computation of first- and second-order corrections to the spread's variance.
- Visual validation of pricing accuracy through **smile comparisons** between model and market or Monte Carlo.

## 🛠️ Requirements

- [Wolfram Mathematica](https://www.wolfram.com/mathematica/) 12.0 or later recommended.
- Most notebooks assume symbolic computation and plotting capabilities.
- Some scripts output `.pdf` snapshots for easier sharing.

## ✅ Recommended Usage

1. Open `BiSABR_Demonstration.nb` to understand the core derivation of the spread variance formula.
2. Use `BISABR_Example.pdf` to see how the formula behaves under different parameterizations.
3. Refer to `BiSABR_MonteCarlo.pdf` for MC benchmarking.
4. Study `spreadoption_sabr2.pdf` to learn how to calibrate cross-correlations from observed spread option data.

## 📌 Notes

- All outputs have been cross-checked with analytical and numerical methods.
- The notebooks may be exported to Python or C++ for real-time pricing engines.

---

