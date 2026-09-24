# QCID — Quantum Consciousness Interface to Higher Dimensions

**Author:** Nasir Khan, Wana, South Waziristan, Pakistan | Nasirk684@gmail.com
**Concept DOI (8-Paper Series):** 10.5281/zenodo.22896411
**Dataset DOI (QCID-II):** 10.5281/zenodo.22581218

This repo contains QCID 8-Paper Series + QCID-II Benchmark Dataset + Quantum Simulation.

### Timeline (Priority Proof)
- V4.2 f00586d — 23 Sep 2026: Simulation seed — BEFORE LIGO O5
- V5.0 — 24 Sep 2026: Paper-1 — 4D Electrodynamics I∝1/r³ law
- V5.1-V5.7: Papers 2-8 upcoming

### Paper-1: QCID Principle
File: Paper-1-QCID-4D-Electrodynamics-Sep3-2026.pdf
Result: Maxwell extended to 4D (x,y,z,w). Wave eq (∇²₄ - 1/c² ∂²/∂t²)E=0. Radiation I_4D ∝ 1/r³ vs I_3D ∝ 1/r². Falsifiable via photonic metamaterials. Simulation 16⁴ grid via Trotterization on NISQ.

### QCID-II Dataset
Benchmark dataset for stability selection of 3 spatial dimensions. 50000 samples, NPZ format, 70/15/15 split. Input: 3D spatial grid, Target: Stability class/score.

Quick Start:
import numpy as np
data = np.load('qcid2_train.npz')
X_train, y_train = data['X'], data['y']

Full Dataset: https://doi.org/10.5281/zenodo.22581218
License: CC BY 4.0

### Citation
Series: Khan, N. (2026). QCID Series. Zenodo. https://doi.org/10.5281/zenodo.22896411
Dataset: @dataset{khan2026qcid2, author={Khan, Nasir}, title={QCID-II}, year={2026}, doi={10.5281/zenodo.22581218}}
