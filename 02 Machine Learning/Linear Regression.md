---
tags:
  - ml/supervised
  - ml/regresi
aliases:
  - Regresi Linear
date: 2026-04-28
status: complete
---

# Linear Regression

> **Ringkasan:** Memodelkan hubungan linier antara fitur dan target kontinu.

## Rumus

`y = beta_0 + beta_1*x_1 + beta_2*x_2 + ... + epsilon`

## Asumsi

1. Linearitas
2. Independensi residual
3. [[Heteroskedastisitas|Homoskedastisitas]]
4. Normalitas residual
5. Tidak ada [[Multicollinearity]]

## Metrik Evaluasi

- [[R-Squared]], [[MAE]], [[MSE]], [[RMSE]]

## Hubungan dengan Konsep Lain

- Terkait: [[Logistic Regression]], [[Regularisasi]], [[Gradient Descent]]
- Library: [[Scikit-Learn]], [[Statsmodels]]