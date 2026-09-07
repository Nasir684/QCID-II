# QCID-II: The Stability Selection of Three Spatial Dimensions

QCID-II is a benchmark dataset for analyzing stability and selection criteria across three spatial dimensions in computational physics and machine learning. This dataset is designed to accelerate research in dimensional stability analysis, spatial modeling, and physics-informed ML.

## 📦 Download & DOI
**Full Dataset**: https://doi.org/10.5281/zenodo.22581218
**DOI**: 10.5281/zenodo.22581218
**License**: [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## 🔬 Motivation & Background
The stability of systems across three spatial dimensions is a fundamental problem in physics and computational modeling. However, there is no standardized dataset to benchmark ML models for dimensional stability selection. QCID-II provides a clean, versioned dataset with ground truth stability labels for 3D spatial systems.

## 📊 Dataset Specifications
- **Version**: 2.0
- **Format**: NPZ
- **Total Samples**: 50000
- **Data Split**: 70/15/15
- **Input Features**: 3D spatial grid with physical parameters
- **Target Variable**: Stability class / Stability score
- **Domains**: Computational Physics, Machine Learning, 3D Spatial Analysis

## 🧪 Benchmark Tasks
1. **Stability Classification**: Classify if a 3D configuration is stable or unstable
2. **Stability Regression**: Predict the stability score of a spatial configuration

Baseline models and example notebooks are provided.

## 🚀 Quick Start
```python
import numpy as np
data = np.load('qcid2_train.npz')
X_train, y_train = data['X'], data['y']
print(f"Dataset loaded: {X_train.shape[0]} samples")
