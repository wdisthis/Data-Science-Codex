---
tags:
  - ml/supervised
aliases:
  - Pohon Keputusan
date: 2026-04-28
status: complete
---

# Decision Tree

> **Ringkasan:** Membagi data secara rekursif berdasarkan fitur yang paling informatif.

## Cara Kerja

Memilih fitur terbaik berdasarkan:
- **Gini Impurity** (CART)
- **Information Gain / Entropy** (ID3, C4.5)

## Kelebihan

- Mudah diinterpretasi dan divisualisasi
- Tidak perlu [[Normalisasi vs Standarisasi|normalisasi]]
- Handle data numerik dan kategorikal

## Kekurangan

- Sangat rentan [[Overfitting]]

## Hubungan dengan Konsep Lain

- Terkait: [[Random Forest]], [[Gradient Boosting]], [[Ensemble Methods]]