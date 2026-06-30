# Self-Optimal Clustering (SOC)

A Python implementation of the **Self-Optimal Clustering (SOC)** algorithm proposed in the IEEE Systems Journal paper *"Self-Optimal Clustering Technique Using Optimized Threshold Function"*.

SOC is an improved clustering algorithm that enhances Improved Mountain Clustering (IMC) by automatically optimizing the threshold function using **Lagrange interpolation**, resulting in better cluster compactness and separation.

---

## Features

- Automatic threshold optimization
- Improved cluster quality over traditional IMC
- Supports arbitrary-dimensional datasets
- Uses silhouette-based optimization
- Determines optimal clustering with iterative refinement
- Suitable for image segmentation and general clustering tasks

---

## Algorithm Overview

The algorithm performs the following steps:

1. Normalize the dataset.
2. Compute an initial threshold.
3. Calculate mountain potentials.
4. Select cluster centers.
5. Form clusters using the threshold.
6. Compute silhouette scores.
7. Optimize the threshold using Lagrange interpolation.
8. Repeat until convergence.

## Installation

```bash
git clone https://github.com/yourusername/self-optimal-clustering.git

cd self-optimal-clustering

pip install -r requirements.txt
```

---

## Usage

```bash
python src/main.py
```

Or inside Python:

```python
from clustering import SOC

model = SOC()
labels = model.fit_predict(data)
```

---

## Evaluation Metrics

The implementation evaluates clustering quality using:

- Global Silhouette Index (GSI)
- Dunn Index
- Partition Index
- Separation Index

Higher GSI and Dunn Index indicate better clustering, while lower Partition and Separation Indices indicate better cluster quality. :contentReference[oaicite:1]{index=1}

---

## Results

Compared with:

- K-Means
- Fuzzy C-Means (FCM)
- Expectation Maximization (EM)
- K-Medoids
- Improved Mountain Clustering (IMC)

SOC consistently achieves improved cluster compactness and separation through optimized threshold selection. :contentReference[oaicite:2]{index=2}

---

## Applications

- Image segmentation
- Pattern recognition
- Medical imaging
- Computer vision
- Unsupervised learning
- Data mining

---

## Reference

N. K. Verma and A. Roy,
**"Self-Optimal Clustering Technique Using Optimized Threshold Function,"**
IEEE Systems Journal, Vol. 8, No. 4, 2014. :contentReference[oaicite:3]{index=3}

---

## License

This project is intended for educational and research purposes.
Please cite the original paper if you use or extend this implementation.
