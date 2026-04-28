# Oxygen-relative ERC Model

This repository contains a minimal dynamical framework exploring recoverability-constrained behavior across 118 chemical elements, parameterized by oxygen-relative geometry.

## Core idea

The model tests whether dynamical accessibility is determined solely by geometric proximity in chemical space, or whether recoverability constraints introduce structured regimes.

Rather than focusing on static properties, the system evaluates how elements respond to transient forcing and whether trajectories remain dynamically accessible.

## Model

We use a minimal recoverability model governed by:

dv/dt = (1 - v)/τ_r - E(t)

where E(t) is a Gaussian forcing term with controlled amplitude and duration.

Each element is embedded into this framework through oxygen-relative geometric scaling, defining:

- r_core: intrinsic recovery scale  
- r_boundary: collapse threshold  

Two operational transitions are tracked:

- **damage onset**: deviation from recoverable dynamics  
- **non-return**: crossing of collapse boundary  

Dynamical regimes are defined based on the ordering of these transitions.

## Results

Across 118 elements, we observe:

- Emergence of distinct dynamical regimes  
- Clustering not explained by linear distance to oxygen  
- Weak correlation between distance and accessibility (r ≈ -0.16)  
- Loss of structure under shuffled control  

These findings suggest that oxygen-relative chemical space may encode structured dynamical accessibility regimes.

## Repository structure

- `notebooks/` — main simulation notebook  
- `data/input/` — input datasets  
- `data/output/` — generated results  
- `figures/` — figures used in the paper  
- `paper/` — manuscript PDF

## Reproducibility

To reproduce the results:

1. Open `notebooks/Periodic_ERC_Model.ipynb` in Google Colab  
2. Run all cells sequentially  
3. All figures and outputs will be generated automatically

No external dependencies beyond standard Python scientific libraries are required.

## Statement

These results suggest that oxygen-relative chemical space may contain a hidden dynamical structure, visible through recoverability pathways rather than static distance alone.
