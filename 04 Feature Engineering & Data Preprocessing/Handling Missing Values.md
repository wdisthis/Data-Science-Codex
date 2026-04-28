---
tags:
  - feature-engineering/cleaning
aliases:
  - Missing Data
  - Imputasi
date: 2026-04-28
status: complete
---

# Handling Missing Values

> **Ringkasan:** Teknik menangani data yang hilang dalam dataset.

## Strategi

| Teknik | Deskripsi | Kapan |
|--------|-----------|-------|
| **Deletion** | Hapus baris/kolom | Missing < 5% |
| **Mean/Median/Mode** | Isi dengan statistik | Sederhana, cepat |
| **KNN Imputation** | Isi berdasarkan tetangga | Lebih akurat |
| **Model-based** | Prediksi dengan ML | Paling akurat, paling lambat |

> [!TIP]
> Median lebih robust untuk data skewed ([[Skewness]]).

## Hubungan dengan Konsep Lain

- Terkait: [[Data Cleaning]], [[Outlier]], [[Pandas]]