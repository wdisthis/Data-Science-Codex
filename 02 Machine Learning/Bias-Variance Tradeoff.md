---
tags:
  - ml/fundamental
aliases:
  - Bias Variance
date: 2026-04-28
status: complete
---

# Bias-Variance Tradeoff

> **Ringkasan:** Keseimbangan antara kesederhanaan model (bias) dan sensitivitasnya terhadap data (variance).

## Definisi

- **Bias:** Kesalahan akibat asumsi model yang terlalu sederhana â†’ [[Underfitting]]
- **Variance:** Sensitivitas model terhadap fluktuasi data training â†’ [[Overfitting]]
- **Total Error** = Bias^2 + Variance + Irreducible Noise

## Diagram

```
       Error
         |        Variance
         |       /
         |      /
  Total  |----/------
  Error  |   / \
         |  /   \
         | /     Bias
         |/
         +-------------------> Model Complexity
```

## Tujuan

Menemukan titik keseimbangan di mana total error minimum.

## Hubungan dengan Konsep Lain

- Terkait: [[Overfitting]], [[Underfitting]], [[Regularisasi]], [[Cross Validation]]