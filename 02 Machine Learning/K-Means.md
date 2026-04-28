---
tags:
  - ml/unsupervised
  - ml/clustering
aliases:
  - K-Means Clustering
date: 2026-04-28
status: complete
---

# K-Means

> **Ringkasan:** Membagi data ke K cluster dengan meminimalkan inertia (jarak dalam cluster).

## Algoritma

1. Inisialisasi K centroid secara acak
2. Assign setiap titik ke centroid terdekat
3. Update centroid ke rata-rata cluster
4. Ulangi hingga konvergen

## Cara Pilih K

- **Elbow Method:** Plot inertia vs K, cari siku
- **[[Silhouette Score]]:** Ukur kualitas clustering

## Kelemahan

- Harus tentukan K di awal
- Sensitif terhadap inisialisasi â†’ gunakan k-means++
- Asumsi cluster berbentuk bola

## Hubungan dengan Konsep Lain

- Terkait: [[DBSCAN]], [[Hierarchical Clustering]], [[Customer Segmentation]]
- Library: [[Scikit-Learn]]