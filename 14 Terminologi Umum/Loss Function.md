---
tags:
  - terminologi
  - ml/fundamental
aliases:
  - Fungsi Loss
  - Cost Function
  - Objective Function
date: 2026-04-28
status: complete
---

# Loss Function

> **Ringkasan:** Fungsi yang mengukur seberapa salah prediksi model â€” yang dioptimalkan selama training.

## Loss Function Umum

| Loss | Task | Rumus Singkat |
|------|------|---------------|
| **MSE** | Regresi | [[MSE]] |
| **Cross-Entropy** | Klasifikasi biner | -[y*log(p) + (1-y)*log(1-p)] |
| **Categorical CE** | Klasifikasi multi-kelas | -SUM(yi * log(pi)) |

## Hubungan dengan Konsep Lain

- Terkait: [[Gradient Descent]], [[Backpropagation]], [[Optimizer]]
- Metrik evaluasi: [[MSE]], [[Log Loss]], [[MAE]]