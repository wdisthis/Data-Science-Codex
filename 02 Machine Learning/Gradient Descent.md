---
tags:
  - ml/fundamental
aliases:
  - GD
  - SGD
  - Stochastic Gradient Descent
date: 2026-04-28
status: complete
---

# Gradient Descent

> **Ringkasan:** Algoritma optimasi yang iteratif menggerakkan parameter ke arah yang menurunkan [[Loss Function]].

## Update Rule

`theta = theta - alpha * nabla_J(theta)`

(alpha = [[Learning Rate]])

## Varian

| Varian | Data per Iterasi | Karakteristik |
|--------|-----------------|---------------|
| **Batch GD** | Semua data | Stabil tapi lambat |
| **SGD** | 1 sampel | Cepat tapi noisy |
| **Mini-batch GD** | Subset (32, 64, 128) | Keseimbangan terbaik |

## Hubungan dengan Konsep Lain

- Terkait: [[Loss Function]], [[Learning Rate]], [[Backpropagation]]
- Optimizer lanjutan: [[Adam]], [[Optimizer]]
- Matematika: [[Turunan dan Gradien]]