# QCID-II: Quantum Cellular Intelligence Dataset v2

QCID-II is a benchmark dataset for developing and evaluating machine learning models on Quantum Cellular Automata (QCA) systems. This dataset is designed to accelerate research in quantum-inspired machine learning, physics simulation, and computational modeling of quantum systems.

## 📦 Download & DOI
**Full Dataset**: https://doi.org/10.5281/zenodo.22581218
**DOI**: 10.5281/zenodo.22581218
**License**: [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## 🔬 Motivation & Background
Quantum Cellular Automata extend classical cellular automata to quantum mechanical systems. They are a promising model for quantum computation and physics simulation. However, the lack of standardized, open datasets has slowed ML research in this domain. QCID-II addresses this by providing a clean, versioned dataset with defined tasks and evaluation metrics.

## 📊 Dataset Specifications
- **Version**: 2.0
- **Format**: [CSV / NPZ]
- **Total Samples**: [X]
- **Data Split**: [Train/Val/Test e.g. 70/15/15]
- **Input Features**: [e.g. Quantum state amplitudes, Cell grid configurations]
- **Target Variable**: [e.g. Next state prediction / Energy classification]
- **Domains**: Quantum Physics, Machine Learning, Cellular Automata

## 🧪 Benchmark Tasks
1. **State Evolution Prediction**: Predict the next state of a QCA system
2. **Pattern Classification**: Classify quantum cellular patterns

Baseline models and example notebooks are provided.

## 🚀 Quick Start
```python
import numpy as np
data = np.load('qcid2_train.npz')
X_train, y_train = data['X'], data['y']
