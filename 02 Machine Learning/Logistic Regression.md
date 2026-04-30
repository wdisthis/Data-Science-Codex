---
tags:
  - ml/supervised
  - ml/klasifikasi
aliases:
  - Regresi Logistik
date: 2026-04-28
status: complete
---

# Logistic Regression

> **Ringkasan:** Klasifikasi biner menggunakan fungsi sigmoid. Bukan regresi sebenarnya!

## Fungsi Sigmoid

$$\sigma(z) = \frac{1}{1 + e^{-z}}$$

> [!NOTE]
> Namanya menyesatkan â€” ini adalah algoritma **klasifikasi**, bukan regresi.

## Hubungan dengan Konsep Lain

- Terkait: [[Linear Regression]], [[Activation Function|Sigmoid]]
- Evaluasi: [[AUC-ROC]], [[Confusion Matrix]], [[Log Loss]]
- Library: [[Scikit-Learn]]