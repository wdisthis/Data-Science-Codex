---
tags:
  - ml/fundamental
aliases:
  - Regularization
  - L1
  - L2
  - Lasso
  - Ridge
date: 2026-04-28
status: complete
---

# Regularisasi

> **Ringkasan:** Teknik mencegah [[Overfitting]] dengan menambahkan penalti pada kompleksitas model.

## Tipe

| Tipe | Penalti | Efek |
|------|---------|------|
| **L1 (Lasso)** | lambda * SUM(abs(wi)) | Beberapa bobot menjadi 0 â†’ [[Feature Selection]] otomatis |
| **L2 (Ridge)** | lambda * SUM(wi^2) | Semua bobot mengecil, tidak pernah nol |
| **Elastic Net** | Kombinasi L1 + L2 | Keseimbangan keduanya |

## Hubungan dengan Konsep Lain

- Terkait: [[Overfitting]], [[Bias-Variance Tradeoff]], [[Feature Selection]]
- Lihat juga: [[Dropout]] (regularisasi di deep learning)