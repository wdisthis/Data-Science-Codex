---
tags:
  - ml/supervised
aliases:
  - Support Vector Machine
date: 2026-04-28
status: complete
---

# SVM

> **Ringkasan:** Mencari hyperplane dengan margin terbesar antara kelas.

## Kernel Trick

Memetakan data ke dimensi lebih tinggi agar bisa dipisahkan secara linier.

| Kernel | Karakteristik |
|--------|---------------|
| Linear | Data linearly separable |
| RBF (Gaussian) | Paling umum, non-linear |
| Polynomial | Non-linear, degree bisa diatur |

## Catatan

- Perlu [[Normalisasi vs Standarisasi|Feature Scaling]]
- Kurang cocok untuk dataset sangat besar

## Hubungan dengan Konsep Lain

- Terkait: [[Logistic Regression]], [[KNN]], [[Feature Scaling]]
- Library: [[Scikit-Learn]]