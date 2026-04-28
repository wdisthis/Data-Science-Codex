---
tags:
  - deep-learning/fondasi
aliases:
  - Backprop
date: 2026-04-28
status: complete
---

# Backpropagation

> **Ringkasan:** Algoritma untuk menghitung gradien [[Loss Function]] terhadap setiap weight menggunakan chain rule.

## Proses

1. **Forward pass** â†’ hitung output
2. **Hitung loss** â†’ bandingkan dengan target
3. **Backward pass** â†’ hitung gradien tiap layer
4. **Update weight** â†’ via [[Gradient Descent]] / [[Optimizer]]

## Hubungan dengan Konsep Lain

- Terkait: [[Gradient Descent]], [[Loss Function]], [[Turunan dan Gradien]]
- Masalah: [[Vanishing Gradient]]