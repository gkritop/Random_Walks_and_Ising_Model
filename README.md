# Random_Walks_and_Ising_Model

## Overview

This project investigates stochastic processes through two main parts: modeling diffusion using random walks, and studying phase transitions in the 2D Ising model using the Metropolis algorithm. Numerical simulations illustrate key concepts in statistical mechanics and thermodynamics.

Part of the **Computational Physics** course at the **Physics Department, University of Crete**.

## Problem Statement

- Model diffusion microscopically via 2D random walks, verifying how the mean squared displacement evolves with time consistent with Fick’s laws.
- Simulate the 2D Ising model to explore thermodynamic properties, such as energy, magnetization, heat capacity, and susceptibility, and study phase transitions near the Curie temperature.

## Methodology

- Implemented 2D and 3D random walk where particles take unit-length steps in random directions, averaging results over multiple trials.
- Simulated the Ising model on a square lattice with nearest-neighbor interactions using the Metropolis Monte Carlo algorithm.
- Calculated thermodynamic observables via importance sampling of spin configurations.
- Applied periodic boundary conditions and used efficient indexing for lattice neighbors.
- Allowed for both ferromagnetic (J > 0) and antiferromagnetic (J < 0) interactions, as well as external magnetic fields.

### Implementation

- Generated random walk trajectories and computed root-mean-square displacement versus number of steps.
- Initialized spin configurations with “cold start” or “hot start” methods.
- Used Metropolis acceptance criteria to sample spin configurations and compute expectation values.
- Applied thermalization to ensure equilibrium before measuring observables.
- Skipped correlated samples to improve statistical accuracy.

## Results

- Random walk simulations confirmed the RMS displacement grows proportional to the square root of the number of steps.
- The Ising model simulations reproduced the phase transition behavior, showing changes in magnetization and energy near the Curie temperature.
- Observed how external magnetic fields affect the critical temperature.
- Visualized spin configurations at temperatures below, near, and above the critical point.

## Conclusion

- The random walk model effectively captures diffusion dynamics consistent with theoretical predictions.
- The Metropolis algorithm successfully simulates phase transitions in the 2D Ising model.
- Results align well with known theoretical behavior, demonstrating key principles of stochastic dynamics and statistical mechanics.
- The approach can be extended to study antiferromagnetism and more complex lattice systems.

## Usage

All code and simulations are contained in the notebook `Stochastic_Physics_Project.ipynb`. Requires Python with NumPy and Matplotlib. Run in any Jupyter environment.

## Acknowledgements

Developed by **Giorgos Kritopoulos** for the Computational Physics course, Physics Department, University of Crete.  
Date: May 13, 2025
