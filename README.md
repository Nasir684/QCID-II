# QCID-II: Quantum Cellular Intelligence Dataset v2

QCID-II is a benchmark dataset for developing and evaluating machine learning models on Quantum Cellular Automata (QCA) systems. It provides standardized data to accelerate research in quantum-inspired ML, physics simulation, and pattern recognition in discrete quantum systems.

## 📦 Download & DOI
**Full Dataset**: https://doi.org/10.5281/zenodo.22581218
**License**: [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## 🔬 Motivation
Training ML models on Quantum Cellular Automata is difficult due to the lack of open, versioned datasets. QCID-II fills this gap by providing clean, documented data with clear benchmark tasks for the research community.

## 📊 Dataset Details
- **Version**: 2.0
- **Format**: [CSV / NPZ]
- **Total Samples**: [X]
- **Input**: [e.g. Quantum state vectors / Cell grid configurations]
- **Target**: [e.g. Next state prediction / Classification]
- **Domain**: Quantum Physics, Machine Learning, Cellular Automata

## 🧪 Benchmark Tasks
1. **State Prediction**: Predict the next QCA state from current state
2. **Classification**: Classify quantum patterns into categories

Example notebooks and baseline code are included.

## 🚀 Quick Start
```python
import pandas as pd

df = pd.read_csv('qcid2_sample.csv')
print(df.head())
