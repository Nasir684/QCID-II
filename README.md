# QCID — Quantum Consciousness Interface to Higher Dimensions

Author: Nasir Khan, Wana, South Waziristan, Pakistan | nasirk684@gmail.com
Concept DOI (8-Paper Series): 10.5281/zenodo.22896411
Dataset DOI (QCID-II): 10.5281/zenodo.22581218
License: CC BY 4.0

This repository is the official archive for the QCID 8-Paper Series + QCID-II Benchmark Dataset + Quantum Simulation Code.

Priority Timeline — GitHub Verifiable
V4.2 f00586d — 23 Sep 2026: Simulation seed + QCID-II scaffold — BEFORE LIGO O5
V5.0-paper1 — 24 Sep 2026: Paper-1 — 4D Electrodynamics I ∝ 1/r³
V5.1-paper2 — 24 Sep 2026: Paper-2 — Gravitational Instability in 4D F ∝ 1/r³
V5.2-V5.7: Papers 3-8 upcoming

Paper Series — Under Concept DOI 10.5281/zenodo.22896411
V5.0 | Paper-1: QCID-I | Paper-1-QCID-4D-Electrodynamics-Sep3-2026.pdf | Maxwell in 4D (x,y,z,w): (∇²₄ - 1/c² ∂²/∂t²)E=0. Gauss flux over 3-sphere area 2π²r³ → I_4D ∝ 1/r³ vs I_3D ∝ 1/r². Falsifiable via photonic metamaterials. 16⁴ grid Trotterization.
V5.1 | Paper-2: QCID-II Gravitational Instability in 4D and Necessity of 3D for Life | Paper-2-QCID-Gravitational-Instability-4D-1-over-r3-Sep3-2026.pdf | Gauss Law in 4D: F_4D(r) = -G_4D*M*m / r³ Eq1, V_4D(r) ∝ 1/r². Circular orbit mv²/r = G_4D*M*m / r³ → v² ∝ 1/r² Eq2. Bertrand's Theorem only V∝1/r and V∝r² give stable closed orbits. Our V∝1/r² → unstable → no planets/stars/galaxies in 4D. QCID must be informational only. Anthropic proof for 3D [Ehrenfest 1921].

Full Derivation — Paper-2
Eq1 — 4D Gravity: In 3D flux over 4πr² → F ∝ 1/r². In 4D flux over 2π²r³ → F_4D(r) = -G_4D*M*m / r³, V_4D(r) ∝ 1/r²
Eq2 — Instability: mv²/r = G_4D*M*m / r³ → v² ∝ 1/r². Bertrand: Only V∝1/r and V∝r² stable. Our V∝1/r² NOT stable → no stable systems.

QCID-II Dataset — DOI 10.5281/zenodo.22581218
Size: 50000 samples, NPZ, 70/15/15 split, Input: 3D grid, Target: Stability score, License: CC BY 4.0, Full: https://doi.org/10.5281/zenodo.22581218
Quick Start: import numpy as np; data = np.load('qcid2_train.npz'); X_train, y_train = data['X'], data['y']

Quantum Simulation Code V4.2 f00586d
import numpy as np; GRID=16
def laplacian_4d(field): lap=np.zeros_like(field); [lap.__iadd__(np.roll(field,-1,axis=a)+np.roll(field,1,axis=a)-2*field) for a in range(4)]; return lap
def intensity_4d(r): return 1.0/(r**3)
def gravity_4d(r,G4D=1.0,M=1.0,m=1.0): return -G4D*M*m/(r**3)
def potential_4d(r): return 1.0/(r**2)

Repo Structure: / Paper-1-QCID-4D-Electrodynamics-Sep3-2026.pdf / Paper-2-QCID-Gravitational-Instability-4D-1-over-r3-Sep3-2026.pdf / qcid2_train.npz / simulation/qcid_4d_trotter.py / README.md / LICENSE

Citation: Khan, N. (2026). QCID — Quantum Consciousness Interface to Higher Dimensions (8-Paper Series). Zenodo. https://doi.org/10.5281/zenodo.22896411
Dataset citation: @dataset{khan2026qcid2, author={Khan, Nasir}, title={QCID-II Benchmark Dataset}, year={2026}, doi={10.5281/zenodo.22581218}}

References: J. Bertrand 1873, P. Ehrenfest 1921, N. Khan 2026[1][2][3]

Note: Papers re-released under Concept DOI 10.5281/zenodo.22896411, Dataset DOI 10.5281/zenodo.22581218 remains distinct. Priority V4.2 f00586d 23 Sep 2026.
