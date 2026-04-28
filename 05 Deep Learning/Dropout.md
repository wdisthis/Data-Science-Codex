---
tags:
  - deep-learning/teknik
date: 2026-04-28
status: complete
---

# Dropout

> **Ringkasan:** Teknik [[Regularisasi]] di mana neuron secara acak dimatikan selama training.

## Cara Kerja

- Setiap neuron dimatikan dengan probabilitas p (biasanya 0.2-0.5)
- Memaksa network belajar representasi yang lebih robust

> [!NOTE]
> Dropout hanya aktif saat **training**, tidak saat inferensi.

## Hubungan dengan Konsep Lain

- Terkait: [[Regularisasi]], [[Overfitting]], [[Batch Normalization]], [[Neural Network]]