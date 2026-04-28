---
tags:
  - ml/supervised
  - ml/ensemble
aliases:
  - GBM
  - GBDT
date: 2026-04-28
status: complete
---

# Gradient Boosting

> **Ringkasan:** Membangun tree secara sekuensial â€” setiap tree memperbaiki kesalahan tree sebelumnya.

## Cara Kerja

1. Latih tree pertama
2. Hitung residual (error)
3. Latih tree berikutnya untuk memprediksi residual
4. Ulangi hingga n_estimators tercapai

## Perbedaan dari Random Forest

- [[Random Forest]] = paralel ([[Bagging]])
- Gradient Boosting = sekuensial ([[Boosting]])

## Hyperparameter Penting

`learning_rate`, `n_estimators`, `max_depth`, `subsample`

## Implementasi Populer

- [[XGBoost]], [[LightGBM]], [[CatBoost]]

## Hubungan dengan Konsep Lain

- Terkait: [[Decision Tree]], [[Boosting]], [[Ensemble Methods]]