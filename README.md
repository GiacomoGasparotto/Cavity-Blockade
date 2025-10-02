# Cavity Blockade Simulation

This repository contains the code and analysis developed for the study of the **cavity blockade effect** in cavity quantum electrodynamics (QED). The project was carried out as part of the course *Quantum Information with Atoms and Photons*.

## Overview

The **cavity blockade** is a quantum phenomenon in which a single photon inside a cavity prevents the absorption of a second one. This effect arises from the anharmonicity of energy levels in the coupled atom–cavity system and is a key ingredient for quantum technologies relying on single-photon sources and quantum gates.

This project investigates the optimal conditions to observe the blockade effect by modeling and simulating the system using the **Jaynes–Cummings Hamiltonian** and solving the **Lindblad master equation** with the [QuTiP](https://qutip.org/) library.

## Main Contributions

- **Hamiltonian model**  
  - Derived from the Jaynes–Cummings interaction between a two-level atom and a single cavity mode.  
  - Included coherent driving and dissipation channels (atomic decay Γ, cavity loss κ).  

- **Numerical simulations**  
  - Solved the Lindblad master equation in the steady state.  
  - Investigated the photon number distribution and temporal dynamics.  
  - Verified the transition between weak- and strong-coupling regimes.  

- **Key results**  
  - Without atom–cavity coupling: observed coherent Poissonian photon statistics.  
  - With strong coupling: demonstrated energy level splitting into dressed states, leading to photon blockade.  
  - Identified parameter regimes (ε, Γ, κ, g̃) favoring single-photon occupancy.  
  - Calculated the second-order correlation function **g²(0) = 0.53**, confirming **antibunching** and effective photon blockade.  

- **Parameter tuning**  
  - Explored how varying drive strength, decay rates, and coupling modifies the mean photon number.  
  - Found that increasing ε to the order of decay rates can enhance single-photon occupation.  

## Methods & Tools

- **Hamiltonian approach**: Jaynes–Cummings model in the rotating wave approximation.  
- **Numerical solver**: Lindblad master equation (QuTiP).  
- **Analysis**: photon statistics, temporal evolution, correlation functions.  

## References

1. Kevin M. Birnbaum, Andreea Boca, Russell Miller, Allen D. Boozer, Tracy E. Northup, and H. Jeff Kimble. *Photon blockade in an optical cavity with one trapped atom*. **Nature**, 436(7047):87–90, 2005.  
2. Christoph Hamsen, Karl Nicolas Tolazzi, Tatjana Wilk, and Gerhard Rempe. *Two-photon blockade in an atom-driven cavity QED system*. **Physical Review Letters**, 118(13):133604, 2017.