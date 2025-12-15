# Drosophila Connectome Network Analysis

**Author**: Kshamaa  
**Date**: December 2024  
**Purpose**: Demonstration of network and spatial analysis methods for neural connectome data

## Overview
This project demonstrates key analytical methods for connectome analysis:
- **Community detection** using modularity maximization (Louvain) and label propagation
- **Spatial distribution analysis** using K-nearest neighbors, Hopkins statistic, and Ripley's K function
- **Multi-scale analysis** comparing network structure and spatial organization across communities

## Methods Implemented

### 1. Community Detection
- Louvain algorithm (greedy modularity maximization)
- Label propagation (SBM-style approach)
- Modularity comparison and validation

### 2. Spatial Analysis
- K-nearest neighbor distance distributions
- Hopkins statistic for clustering detection
- Ripley's K and L functions for multi-scale pattern analysis
- Community-specific spatial distributions

### 3. Code Optimization
- Vectorized operations using NumPy
- Efficient nearest-neighbor search with ball trees
- Memory-efficient processing of large spatial datasets

## Key Results
- Detected **X communities** with modularity score of **Y**
- Synaptic distributions show **[clustered/random]** pattern (Hopkins: Z)
- Communities vary in spatial organization, suggesting functional specialization

## Files
- `connectome_analysis.ipynb`: Main analysis notebook
- `community_detection_louvain.png`: Community structure visualization
- `knn_spatial_analysis.png`: Spatial distribution results
- `ripleys_function.png`: Multi-scale spatial patterns

## Technical Stack
- Python 3.x
- NetworkX (network analysis)
- scikit-learn (KNN, spatial methods)
- SciPy (statistical testing)
- NumPy/Pandas (data manipulation)

## Running the Analysis
```bash
pip install -r requirements.txt
jupyter notebook connectome_analysis.ipynb
```

## References
1. Dorkenwald et al. (2024) "Neuronal wiring diagram of an adult brain" Nature
2. Betzel & Bassett (2017) "Multi-scale brain networks" NeuroImage
```

### **requirements.txt**
```
networkx>=3.0
python-louvain>=0.16
scikit-learn>=1.0
scipy>=1.9
numpy>=1.23
pandas>=1.5
matplotlib>=3.5
seaborn>=0.12
jupyter>=1.0
