---
tags:
  - terminologi
  - statistik/lanjutan
aliases:
  - Multikolinearitas
date: 2026-04-28
status: complete
---

# Multicollinearity

> **Ringkasan:** Dua atau lebih [[Feature]] berkorelasi tinggi satu sama lain.

## Dampak

- Koefisien [[Linear Regression]] menjadi tidak stabil
- Sulit interpretasi kontribusi masing-masing fitur

## Deteksi

- Correlation matrix ([[Heatmap]])
- VIF (Variance Inflation Factor)

## Solusi

- [[Feature Selection]], [[PCA]], [[Regularisasi|Ridge Regression]]

## Hubungan dengan Konsep Lain

- Terkait: [[Linear Regression]], [[Feature Selection]], [[PCA]], [[Korelasi vs Kausalitas]]