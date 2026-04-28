---
tags:
  - ml/supervised
  - ml/ensemble
aliases:
  - RF
date: 2026-04-28
status: complete
---

# Random Forest

> **Ringkasan:** Ensemble dari banyak [[Decision Tree]] menggunakan [[Bagging]].

## Cara Kerja

1. Buat banyak decision tree dari subset data (bootstrap)
2. Setiap tree gunakan subset fitur acak
3. Output: voting mayoritas (klasifikasi) atau rata-rata (regresi)

## Kelebihan

- Robust terhadap [[Overfitting]]
- Handle missing values dengan baik
- Memberikan feature importance

## Hubungan dengan Konsep Lain

- Terkait: [[Decision Tree]], [[Bagging]], [[Ensemble Methods]]
- Bandingkan: [[Gradient Boosting]], [[XGBoost]]
- Library: [[Scikit-Learn]]