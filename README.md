# NumPy Mastery: Comprehensive Guide to Vectorized Computing

A high-performance introduction and reference guide for NumPy (`numpy.ndarray`), the foundation of numerical computing, data science, and machine learning in Python. This repository contains the reference file `numpy_tutorial.ipynb`.

---

## 🏎️ Why NumPy?
Python lists are flexible but slow for mathematical operations due to overhead and dynamic typing. NumPy provides **homogeneous, contiguous memory blocks (`ndarrays`)** combined with **vectorized operations implemented in C**, eliminating slow Python loops.

### Performance Vectorization Metric
* **Array Size:** 1,000,000 elements
* **Python List Addition:** ~0.0356 seconds
* **NumPy Array Addition:** ~0.0010 seconds
* **Speedup:** NumPy is **~35.x - 36.x faster** than pure Python loops.

---

## 🗺️ Core Core Concepts Covered

### 1. Vectorized Operations & Broadcasting
Mathematical and scalar computations executed without loops. Elements are compared or modified element-wise automatically.

### 2. Multi-dimensional Arrays & Axis Mechanics
Understanding structural transformations along specific dimensions:
* `axis=0`: Operations perform downward (collapsing rows, analyzing columns).
* `axis=1`: Operations perform crosswise (collapsing columns, analyzing rows).
* `3D Arrays`: Operations scale across depth (`axis=0`), height (`axis=1`), and width (`axis=2`).

### 3. Slicing & Memory Management (Views vs. Copies)
* **Views:** Slicing arrays (`arr[0:5]`) references the original block memory. Modifying a slice alters the original data.
* **Copies:** Deep allocation via explicit `.copy()` or advanced/fancy indexing generates entirely separate data structures.

---

## 🛠️ Repository File Structure

```text
├── .gitignore               # Excludes standard Python cache, logs, and checkpoints
├── README.md                # Documentation and architectural summary
└── numpy_tutorial.ipynb     # Main executable Jupyter notebook containing code tutorials
