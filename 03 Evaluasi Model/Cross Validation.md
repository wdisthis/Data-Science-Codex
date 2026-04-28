---
tags:
  - evaluasi/validasi
aliases:
  - CV
  - k-Fold
date: 2026-04-28
status: complete
---

# Cross Validation

> **Ringkasan:** Teknik evaluasi model dengan membagi data ke beberapa fold dan merotasi set validasi.

## Tipe

| Tipe | Deskripsi |
|------|-----------|
| **k-Fold CV** | Bagi data ke k subset, rotasi k kali |
| **Stratified k-Fold** | Pastikan proporsi kelas sama di setiap fold ([[Class Imbalance]]) |
| **Leave-One-Out** | k = n. Sangat akurat tapi lambat |

## Mengapa Penting

- Mengurangi [[Overfitting]] saat evaluasi
- Estimasi performa lebih reliable dari single split

## Hubungan dengan Konsep Lain

- Terkait: [[Train-Validation-Test Split]], [[Hyperparameter Tuning]], [[Overfitting]]
- Library: [[Scikit-Learn]]