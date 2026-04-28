---
tags:
  - ml/supervised
aliases:
  - K-Nearest Neighbors
date: 2026-04-28
status: complete
---

# KNN

> **Ringkasan:** Mengklasifikasikan titik baru berdasarkan K tetangga terdekatnya.

## Hyperparameter Utama

- **K (jumlah tetangga):**
  - K kecil â†’ high variance ([[Overfitting]])
  - K besar â†’ high bias ([[Underfitting]])

## Kelemahan

- Lambat untuk dataset besar (lazy learner)
- Sangat sensitif terhadap skala fitur â†’ wajib [[Feature Scaling]]
- Curse of dimensionality

## Hubungan dengan Konsep Lain

- Terkait: [[SVM]], [[Normalisasi vs Standarisasi]], [[Feature Scaling]]
- Library: [[Scikit-Learn]]