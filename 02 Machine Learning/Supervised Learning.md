---
tags:
  - ml/paradigma
  - ml/supervised
aliases:
  - Pembelajaran Terawasi
date: 2026-04-28
status: complete
---

# Supervised Learning

> **Ringkasan:** Paradigma ML di mana model belajar dari data yang memiliki [[Label]] (jawaban yang benar).

## Tipe Task

| Task | Output | Contoh Algoritma |
|------|--------|-----------------|
| **Klasifikasi** | Kategori diskrit | [[Logistic Regression]], [[SVM]], [[Random Forest]] |
| **Regresi** | Nilai kontinu | [[Linear Regression]], [[Gradient Boosting]] |

## Alur Kerja

1. Kumpulkan data berlabel
2. Split: [[Train-Validation-Test Split]]
3. Latih model
4. Evaluasi: [[Confusion Matrix]], [[AUC-ROC]], [[RMSE]]
5. Tuning: [[Hyperparameter Tuning]]

## Hubungan dengan Konsep Lain

- Terkait: [[Unsupervised Learning]], [[Reinforcement Learning]], [[Semi-Supervised Learning]]