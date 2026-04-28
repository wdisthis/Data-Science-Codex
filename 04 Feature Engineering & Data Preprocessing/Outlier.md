---
tags:
  - feature-engineering/cleaning
aliases:
  - Pencilan
  - Anomali
date: 2026-04-28
status: complete
---

# Outlier

> **Ringkasan:** Titik data yang jauh berbeda dari mayoritas data.

## Deteksi

| Metode | Cara |
|--------|------|
| **IQR Method** | Outlier = di luar [Q1 - 1.5*IQR, Q3 + 1.5*IQR] |
| **Z-score** | Outlier = abs(z) > 3 |
| **Isolation Forest** | Algoritma ML untuk [[Anomaly Detection]] |

## Penanganan

- Hapus, cap (winsorizing), transformasi log, atau pertahankan jika informatif.

## Hubungan dengan Konsep Lain

- Terkait: [[Kurtosis]], [[Box Plot]], [[Anomaly Detection]]
- Visualisasi: [[Box Plot]], [[Scatter Plot]]