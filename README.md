# Hybrid Quantum-Classical Pipelines for Drug Discovery

## Overview
This repository demonstrates an integrated computational pipeline for drug discovery, bridging classical chemoinformatics with quantum mechanical simulations. The project explores how the Variational Quantum Eigensolver (VQE) can be utilized to refine molecular leads identified through classical machine learning heuristics.

## Motivation
Molecular docking and electronic structure prediction are computationally expensive. While classical methods excel at high-throughput screening, they often lack the precision required for complex electron correlation problems. This project showcases a "best of both worlds" approach:
1. **Classical Screening**: Rapidly filtering chemical libraries using Random Forest regressors and RDKit descriptors.
2. **Quantum Refinement**: Using PennyLane to perform VQE simulations for high-accuracy ground-state energy calculations.

## Methodologies
- **Classical ML**: Scikit-learn implementation of Random Forest Regressors for predicting binding affinity based on Lipinski descriptors.
- **Quantum Simulation**: VQE implementation using a DoubleExcitation Ansatz.
- **Mapping**: Jordan-Wigner transformation of molecular Hamiltonians into qubit operators.

## Installation and Usage
To run the simulations locally, ensure you have Python 3.8+ installed.

1. Clone the repository:
   ```bash
   git clone https://github.com/abdullahayder29/quantum-drug-discovery.git
