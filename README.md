# PPTSA

> **Precipitation Probabilistic Time Series Analysis**  
> Frequency analysis, statistical learning, and uncertainty-aware forecasting of long-term precipitation records.

[![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-F37626.svg)](https://jupyter.org)
[![Python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![MATLAB](https://img.shields.io/badge/MATLAB-supported-orange.svg)](https://www.mathworks.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](#-license)

---

## 🌧️ Overview

This repository presents a **probabilistic time-series analysis of precipitation**, focusing on the statistical structure, impulse-like behavior, and predictability of rainfall.

Using **140 years of daily precipitation data from Central Park, New York City**, the project combines:

- Frequency-domain analysis  
- Classical stochastic models  
- Point-process formulations  
- Deep learning approaches  
- Probabilistic uncertainty quantification  

The goal is to **understand precipitation dynamics**, assess **forecasting limits**, and **explicitly characterize uncertainty**, particularly in the presence of intermittent and impulsive rainfall events.

---

## 🔬 Methods & Modeling Framework

The repository implements and compares the following approaches:

- **Frequency Domain Analysis**  
  Identifies periodicity (or lack thereof) and highlights challenges introduced by impulse-like precipitation patterns.

- **ARIMAX / SARIMAX Models**  
  Captures trends and conditional dependencies using classical time-series models with exogenous variables.

- **Marked Point Process (MPP)**  
  Models precipitation as an impulse-driven stochastic process, offering physical and statistical intuition beyond Gaussian assumptions.

- **LSTM Neural Networks**  
  Learns temporal dependencies among multiple meteorological variables using tuned deep recurrent architectures.

- **Gaussian Process (GP) Residual Modeling**  
  Quantifies predictive uncertainty by modeling LSTM residuals probabilistically.

---

## 📊 Key Findings (High Level)

- Precipitation exhibits **no strong periodicity**, complicating frequency-based forecasting.
- **ARIMAX/SARIMAX** effectively captures long-term trends but struggles with impulses.
- **Marked Point Processes** provide interpretability for impulse-like rainfall events.
- **LSTM models** capture trends but show limited accuracy for exact daily values.
- **Gaussian Processes** accurately model residual uncertainty, improving probabilistic predictions.

---

## 📁 Repository Structure

```text
PPTSA/
├─ Data/
│  └─ Raw and processed meteorological datasets
│
├─ Figures/
│  └─ Generated plots, diagnostics, and visual summaries
│
├─ Models/
│  ├─ Frequency analysis
│  ├─ ARIMAX / SARIMAX models
│  ├─ Marked Point Process formulations
│  ├─ LSTM implementations
│  └─ Gaussian Process residual models
│
├─ Report/
│  └─ PDF/
│     └─ Paper.pdf
│
├─ README.md
└─ LICENSE

---


## 📬 Contact

For questions, feedback, or collaboration opportunities, please email me at:  
[omid.emamjomehzadeh@nyu.edu](mailto:omid.emamjomehzadeh@nyu.edu)

---

## 📚 Citation

If you use this repository in your research or projects, please cite it as follows.

BibTeX format:

```bibtex
@misc{emamjomehzadeh2025pptsa,
  author       = {Emamjomehzadeh, Omid}, {Ruixuan, Zhang}, {Ahmadreza, Ahmadjou}
  title        = {Daily Rainfall Time Series Analysis of Central Park, New York},
  year         = {2024},
  howpublished = {\url{https://github.com/omidemam/PPTSA}},
}
Copy code






