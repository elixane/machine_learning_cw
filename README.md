# Machine Learning Coursework – Artificial Intelligence

## Overview

This project was developed as part of the second year **Artificial Intelligence** module at Durham University (2024–25 academic year).
It explores the **BraVL multimodal dataset**, which combines **brain, image, and text** features to investigate how machine learning models can interpret and relate information across different modalities.

The project implements a **K-Nearest Neighbours (KNN)** classifier from scratch, conducts **data exploration and visualisation**, and analyses performance through **custom and baseline comparisons**. It also explores the impact of **different train/test splits** on model generalisation.

---

## Key Components

### 1. Data Exploration

* Conducted statistical analysis and visualisation of brain, image, and text modalities.
* Identified class imbalance and correlations using histograms, bar charts, and heatmaps.
* Highlighted the suitability of distance-based models due to low feature correlation.

### 2. Model Implementation

* Built a **custom KNN model** using only core Python libraries (no external ML packages).
* Implemented **Euclidean distance–based classification** and **hyperparameter tuning** for `k`.
* Compared against a baseline sklearn implementation.

### 3. Model Improvement

* Applied preprocessing (MinMax scaling, standardisation, PCA) to enhance performance.
* Introduced **class weighting** to handle imbalance and improve efficiency.
* Achieved an accuracy increase from **55% to 80%** on the full dataset.

### 4. Paradigm Design

* Experimented with multiple data splits (50/50 → 90/10) to analyse model robustness.
* Found that an **80/20 split** provided optimal balance between accuracy and generalisation.

---

## Results Summary

| Model           | Dataset    | Accuracy   | F1-Score   |
| --------------- | ---------- | ---------- | ---------- |
| Baseline KNN    | Whole      | 55.22%     | 50.32%     |
| Baseline KNN    | 20 classes | 68.33%     | 65.89      |
| Improved Custom | Whole      | **80.84%** | **80.69%** |
| Improved Custom | 20 classes | **99.17%** | **99.16%** |

Visualisations (confusion matrices and correlation heatmaps) demonstrate high alignment between predictions and ground truth after model improvements.

---

## Repository Structure

```
├── setup.ipynb          # Jupyter Notebook with full code implementation
├── report.pdf           # Final technical report (arXiv-style)
└── README.md            # Project overview
```

---

## References

Long, Y. (2025). *Multimodal Machine Learning with Brain, Image, and Text Data*.
[Google Colab Starter Code](https://colab.research.google.com/drive/1rejEQTW-J2bh88_DyVvHyboB-chSY0ZS)

