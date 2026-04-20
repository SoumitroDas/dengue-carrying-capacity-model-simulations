# 🦟 Dengue Transmission Model: Impact of Carrying Capacity on Control Strategies

[![DOI](https://img.shields.io/badge/DOI-10.1080/25765299.2026.2651569-blue)](https://doi.org/10.1080/25765299.2026.2651569)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the **Wolfram Mathematica** notebooks and supplementary materials for the research article published in the *Arab Journal of Basic and Applied Sciences* (2026).

## 📋 Overview

Dengue fever, a mosquito-borne viral disease, poses significant public health challenges in tropical and subtropical regions. This study introduces an innovative **SEIR-SEI epidemiological model** that incorporates **mosquito carrying capacity** as a dynamic variable influenced by two key intervention strategies:

- **Waste Management (W)**: Effective waste disposal reduces breeding sites for Aedes mosquitoes.
- **Public Awareness (A)**: Community education campaigns to promote preventive measures.

The model demonstrates how these interventions can drive the **basic reproduction number (R₀)** below 1, achieving disease elimination.

### 🔬 Key Contributions
- **Mathematical Modeling**: SEIR (Susceptible-Exposed-Infectious-Recovered) for humans and SEI for mosquitoes.
- **Carrying Capacity Dynamics**: Mosquito population limited by environmental factors.
- **Intervention Analysis**: Quantitative assessment of waste management and awareness impacts.
- **Numerical Simulations**: Comprehensive analysis of transmission dynamics and control thresholds.

## 📊 Model Diagram

```mermaid
graph TD
    A[Susceptible Humans (S_h)] --> B[Exposed Humans (E_h)]
    B --> C[Infectious Humans (I_h)]
    C --> D[Recovered Humans (R_h)]

    E[Susceptible Mosquitoes (S_m)] --> F[Exposed Mosquitoes (E_m)]
    F --> G[Infectious Mosquitoes (I_m)]

    G --> B
    C --> F

    H[Waste Management (W)] --> I[Carrying Capacity (K)]
    J[Public Awareness (A)] --> I

    I --> G
```

## 📁 Repository Contents

### 1. 📈 Numerical Solution
**File**: `Numerical Solution.nb`

This notebook implements the full nonlinear system of differential equations and provides:
- Time-series plots of all compartments (S_h, E_h, I_h, R_h, S_m, E_m, I_m)
- Phase portraits and trajectory analysis
- Intervention scenario comparisons
- Stability analysis of equilibrium points

### 2. 🎯 R₀ Simulation
**File**: `R0 Simulation.nb`

Explores the basic reproduction number as a function of intervention parameters:
- 3D surface plots of R₀ = f(A, W)
- Contour plots identifying control thresholds
- Sensitivity heatmaps
- Optimal intervention strategies visualization

### 3. 🔍 Sensitivity Analysis
**File**: `Sensitivity Analysis.nb`

Comprehensive parameter sensitivity analysis including:
- Partial rank correlation coefficients (PRCC)
- Tornado diagrams for parameter importance
- Uncertainty quantification
- Identification of most influential model parameters

### 4. 📄 Research Paper
**File**: `Role of carrying capacity in dengue control a mathematical model on waste management and public awareness.pdf`

Full published manuscript with detailed methodology, results, and discussion.

## 🛠️ Requirements & Installation

### Software Prerequisites
- **Wolfram Mathematica** 12.0 or later (recommended)
- **Wolfram Player** (free) for viewing notebooks without full Mathematica license

### Getting Started
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/dengue-carrying-capacity-model.git
   cd dengue-carrying-capacity-model
   ```

2. Open notebooks in Mathematica:
   - Launch Wolfram Mathematica
   - File → Open → Select desired .nb file

3. Evaluate cells sequentially (Shift+Enter) to reproduce results

## 📖 Usage Guide

### Running Simulations
- **Numerical Solution**: Adjust parameter values in the parameter block and re-evaluate
- **R₀ Simulation**: Modify intervention ranges to explore different scenarios
- **Sensitivity Analysis**: Change sample sizes or parameter distributions as needed


## 🎯 Results & Insights

- **Waste Management Impact**: 30% improvement in waste collection can reduce R₀ by up to 40%
- **Awareness Campaigns**: Community education programs show exponential decay in transmission potential
- **Synergistic Effects**: Combined interventions yield multiplicative benefits
- **Threshold Analysis**: Critical intervention levels for disease elimination identified

## 📚 Citation

If you use this code or findings in your research, please cite:

```bibtex
@article{das2026role,
  title={Role of Carrying Capacity in Dengue Control: A Mathematical Model on Waste Management and Public Awareness},
  author={Das, Soumitro Kumar and Maruf, Jabed Hasan},
  journal={Arab Journal of Basic and Applied Sciences},
  year={2026},
  doi={10.1080/25765299.2026.2651569}
}
```

## 👥 Authors & Affiliation

- **Soumitro Kumar Das** - Department of Applied Mathematics, University of Rajshahi
- **Jabed Hasan Maruf** - Department of Applied Mathematics, University of Rajshahi

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

We welcome contributions! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request with detailed description

## 📞 Contact

For questions or collaborations:
- Email: [sdasshuvro@gmail.com](mailto:sdasshuvro@gmail.com)

---

*🦟 Fight dengue through science and community action! 🦟*