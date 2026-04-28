---
tags:
  - ml/fundamental
date: 2026-04-28
status: complete
---

# Overfitting

> **Ringkasan:** Model terlalu menghafal data training sehingga performa buruk pada data baru.

## Tanda-tanda

- Training error sangat rendah
- Test/validation error jauh lebih tinggi

## Penyebab

- Model terlalu kompleks
- Data training terlalu sedikit
- Fitur terlalu banyak

## Solusi

- [[Regularisasi]] (L1/L2)
- [[Dropout]] (deep learning)
- [[Cross Validation]]
- Lebih banyak data
- Simplifikasi model
- [[Early Stopping]]

## Hubungan dengan Konsep Lain

- Terkait: [[Underfitting]], [[Bias-Variance Tradeoff]], [[Learning Curve]]