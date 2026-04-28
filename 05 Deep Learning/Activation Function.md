---
tags:
  - deep-learning/fondasi
aliases:
  - Fungsi Aktivasi
date: 2026-04-28
status: complete
---

# Activation Function

> **Ringkasan:** Fungsi non-linear yang memungkinkan neural network belajar pola kompleks.

## Fungsi Umum

| Fungsi | Rumus | Kegunaan |
|--------|-------|----------|
| **ReLU** | max(0, x) | Hidden layers (paling umum) |
| **Sigmoid** | 1/(1+e^-x) | Output biner ([[Logistic Regression]]) |
| **Softmax** | e^xi / SUM(e^xj) | Output multi-kelas |
| **Tanh** | (e^x - e^-x)/(e^x + e^-x) | Hidden layers, output [-1, 1] |

## Hubungan dengan Konsep Lain

- Terkait: [[Neural Network]], [[Vanishing Gradient]], [[Backpropagation]]