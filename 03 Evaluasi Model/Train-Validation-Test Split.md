---
tags:
  - evaluasi/validasi
aliases:
  - Data Split
  - Train Test Split
date: 2026-04-28
status: complete
---

# Train-Validation-Test Split

> **Ringkasan:** Membagi data menjadi tiga bagian dengan peran berbeda.

## Peran

- **Training set:** Melatih model
- **Validation set:** Tuning [[Hyperparameter Tuning|hyperparameter]] dan pemilihan model
- **Test set:** Evaluasi akhir â€” **HANYA DIGUNAKAN SEKALI!**

## Rasio Umum

`70/15/15` atau `80/10/10`

> [!WARNING]
> Jangan pernah tuning model berdasarkan test set â€” itu menyebabkan [[Data Leakage]].

## Hubungan dengan Konsep Lain

- Terkait: [[Cross Validation]], [[Data Leakage]], [[Overfitting]]