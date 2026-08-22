# Simulation of Surface Plasmon Resonance in two Cesium Nanosphere

This repository contains my undergraduate project report on the plasmonic coupling and localized surface plasmon resonance (LSPR) of cesium (Cs) nanosphere dimers, simulated using the Discrete Dipole Approximation (DDA) method implemented in DDSCAT 7.3.3[cite: 3]. The work investigates how varying nanoparticle radii and inter-particle separation distances affect the extinction spectrum ($Q_{\text{ext}}$)[cite: 3].

The report details the setup of the target geometry configuration (`SPHERES_N`), parameter definitions, and target orientation[cite: 3]. The numerical findings highlight that unlike noble metal dimers (such as gold), cesium nanosphere dimers exhibit minimal plasmonic coupling and maintain a single extinction peak near 700–710 nm across varying separations[cite: 3].

Repository Contents
---
* `Cs_Nanosphere_Simulation_DDSCAT.pdf` — Undergraduate project report covering DDA theory, target file setup, extinction spectra, and LSPR analysis[cite: 3].
* `plotting_Q_ext.py` — Python script for plotting extinction spectra against wavelength for different nanoparticle radii and separation values[cite: 3].

Requirements
---
* Software:
  * DDSCAT 7.3.3[cite: 3]
* Python:
  * NumPy[cite: 3]
  * Matplotlib[cite: 3]
