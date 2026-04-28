---
tags:
  - ml/unsupervised
  - ml/dimensionality-reduction
aliases:
  - Principal Component Analysis
date: 2026-04-28
status: complete
---

# PCA

> **Ringkasan:** Dimensionality reduction dengan mempertahankan variansi maksimum.

## Cara Kerja

1. Standardisasi data
2. Hitung covariance matrix
3. Hitung [[Eigenvalue dan Eigenvector]]
4. Pilih komponen dengan eigenvalue terbesar
5. Proyeksikan data ke ruang baru

## Kapan Digunakan

- Visualisasi data berdimensi tinggi
- Mengurangi [[Multicollinearity]]
- Mempercepat training model

> [!WARNING]
> Komponen PCA tidak bisa diinterpretasikan langsung sebagai fitur asli.

## Hubungan dengan Konsep Lain

- Terkait: [[t-SNE]], [[UMAP]], [[Aljabar Linear]], [[Eigenvalue dan Eigenvector]]
- Perlu: [[Normalisasi vs Standarisasi|Standarisasi]]
- Library: [[Scikit-Learn]]