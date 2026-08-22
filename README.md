# Simulation of Plasmonic Coupling and Surface Plasmon Resonance in Cesium Nanosphere Dimers

Numerical simulation of light scattering, extinction spectra, and localized surface plasmon resonance (LSPR) in two-particle cesium (Cs) nanosphere systems using the Discrete Dipole Approximation (DDA) method implemented in DDSCAT 7.3.3.

---

## Project Overview

Cesium nanoparticles exhibit unique optical properties and strong polarizability in the UV-visible spectrum. This project investigates the plasmonic interaction and extinction coefficient ($Q_{\text{ext}}$) behavior of identical two-sphere cesium dimers across variations in:
1. Nanoparticle radius ($a_0 = 10\text{ nm to } 40\text{ nm}$) for touching spheres.
2. Inter-particle separation distance ($d = 0\text{ to } 12d$, where $d = 1.5\text{ nm}$) for fixed radii ($a_0 = 10\text{ nm}$).

Unlike noble metal nanostructures (e.g., gold dimers) which exhibit pronounced plasmonic coupling and peak splitting due to strong near-field interactions, cesium dimers maintain a single localized resonance peak near $700\text{ nm -- } 720\text{ nm}$, indicating significantly lower plasmonic coupling sensitivity to inter-particle separation.

---

## Method and Computational Setup

* **Framework:** Discrete Dipole Approximation (DDA) via DDSCAT 7.3.3.
* **Target Geometry:** `SPHERES_N` configuration for two identical spheres defined in a custom `.targ` file.
* **Optical Constants:** Complex refractive index values for cesium ($0.5\text{ eV -- } 4.0\text{ eV}$) obtained from N. V. Smith (Phys. Rev. B, 1970).
* **Medium:** Vacuum ($n = 1.00$).
* **Discretization:** Dipole grid spacing fixed at $d = 1.5\text{ nm}$.
* **Wavelength Sweep:** $300\text{ nm to } 1500\text{ nm}$.
* **Wave Propagation & Polarization:** Incident wave propagation along the $\hat{x}$-direction with electric field $E$ polarized along the $\hat{y}$-direction.

---

## Key Findings

### 1. Size-Dependent Extinction Spectra (Touching Spheres)
* **10 nm Radius:** Single peak at $697\text{ nm}$.
* **20 nm Radius:** Single peak at $705\text{ nm}$.
* **30 nm Radius:** Peak at $705\text{ nm}$ with secondary shoulder feature emerging near $1.0\ \mu\text{m}$.
* **40 nm Radius:** Red-shifted peak at $719\text{ nm}$.

### 2. Separation-Dependent Extinction Spectra ($a_0 = 10\text{ nm}$)
* Varying inter-particle distance from $0$ to $12d$ ($18\text{ nm}$) results in minimal peak shift ($697\text{ nm}$ to $709\text{ nm}$).
* The lack of peak splitting or significant field enhancement indicates weak intrinsic plasmonic coupling between cesium nanoparticles compared to gold or silver nanostructures.
