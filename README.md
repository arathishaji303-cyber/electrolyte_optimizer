# Electrolyte Optimizer 

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![PyMatGen](https://img.shields.io/badge/PyMatGen-2023-green)
![XGBoost](https://img.shields.io/badge/XGBoost-R²%3D0.83-orange)
![Materials Project](https://img.shields.io/badge/Data-Materials%20Project-purple)

> A materials informatics pipeline for solid-state battery 
> electrolyte discovery using machine learning.
> ## Project Overview

Solid-state electrolytes (SSEs) are the key bottleneck in next-generation 
battery development. Identifying promising SSE candidates from the vast 
chemical space of known materials is slow and expensive using traditional 
experimental methods.

This project builds a complete materials informatics pipeline that:

- Extracts 21,764 Li-containing materials from the Materials Project API
- Filters to 4,017 validated SSE candidates using domain-driven criteria
- Featurizes crystal structures using Magpie compositional descriptors
- Trains an XGBoost surrogate model to predict band gap (R²=0.83)
- Visualizes the chemical space using UMAP dimensionality reduction

## Key Results

| Metric | Value |
|--------|-------|
| Raw materials queried | 21,764 |
| SSE candidates after filtering | 4,017 |
| Retention rate | 18.4% |
| Surrogate model MAE | 0.328 eV |
| Surrogate model RMSE | 0.487 eV |
| Surrogate model R² | 0.828 |
| Most important features | NValence, Electronegativity |

---

