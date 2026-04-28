---
tags:
  - feature-engineering/scaling
aliases:
  - Normalization
  - Standardization
  - Z-score
  - Min-Max
date: 2026-04-28
status: complete
---

# Normalisasi vs Standarisasi

> **Ringkasan:** Dua teknik scaling fitur agar algoritma bekerja optimal.

## Perbandingan

| Teknik | Rumus | Hasil | Kapan Digunakan |
|--------|-------|-------|-----------------|
| **Min-Max** | (x - min) / (max - min) | [0, 1] | [[KNN]], [[Neural Network]] |
| **Z-score** | (x - mu) / sigma | mean=0, std=1 | [[SVM]], [[PCA]], [[Logistic Regression]] |

> [!TIP]
> Algoritma berbasis jarak **memerlukan** scaling. Tree-based methods ([[Decision Tree]], [[Random Forest]]) **tidak** memerlukannya.

## Hubungan dengan Konsep Lain

- Terkait: [[Feature Scaling]], [[KNN]], [[SVM]], [[PCA]]
- Library: [[Scikit-Learn]]