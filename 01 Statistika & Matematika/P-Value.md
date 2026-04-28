---
tags:
  - statistik/inferensial
aliases:
  - nilai-p
  - p value
date: 2026-04-28
status: complete
---

# P-Value

> **Ringkasan:** Probabilitas mendapatkan hasil yang sama ekstrem (atau lebih ekstrem) dengan data yang diamati, *jika hipotesis nol (H0) benar*.

## Definisi

P-value mengukur seberapa konsisten data yang diamati dengan [[Hipotesis]] nol. Semakin kecil p-value, semakin kuat bukti melawan H0.

## Interpretasi

- `p < 0.05` â†’ Tolak H0 (hasil dianggap signifikan secara statistik)
- `p >= 0.05` â†’ Gagal tolak H0 (tidak cukup bukti melawan H0)

> [!WARNING]
> p-value **BUKAN** probabilitas bahwa H0 benar. Signifikansi statistik â‰  signifikansi praktis.

## Contoh

Uji apakah rata-rata tinggi badan pria dan wanita berbeda â†’ p = 0.02 â†’ ada perbedaan signifikan.

## Hubungan dengan Konsep Lain

- Terkait: [[Hipotesis]], [[Confidence Interval]], [[Type I dan Type II Error]]
- Digunakan di: [[T-Test]], [[ANOVA]], [[Chi-Square Test]], [[A-B Testing]]
- Library: [[Statsmodels]], [[SciPy]]