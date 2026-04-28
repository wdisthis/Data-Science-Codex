---
tags:
  - statistik/inferensial
aliases:
  - Hypothesis Testing
  - Uji Hipotesis
  - H0
  - H1
date: 2026-04-28
status: complete
---

# Hipotesis

> **Ringkasan:** Kerangka formal untuk menguji klaim tentang populasi berdasarkan data sampel.

## Definisi

- **H0 (Null Hypothesis):** Asumsi awal â€” biasanya menyatakan tidak ada efek atau tidak ada perbedaan.
- **H1 (Alternative Hypothesis):** Pernyataan yang ingin dibuktikan â€” kebalikan dari H0.

## Contoh

| Konteks | H0 | H1 |
|---------|----|----|
| Obat baru | Obat tidak berpengaruh | Obat berpengaruh |
| [[A-B Testing]] | Tidak ada perbedaan konversi | Ada perbedaan konversi |

## Proses Uji Hipotesis

1. Tentukan H0 dan H1
2. Pilih tingkat signifikansi (alpha, biasanya 0.05)
3. Hitung statistik uji ([[T-Test]], [[ANOVA]], dll.)
4. Hitung [[P-Value]]
5. Bandingkan p-value dengan alpha â†’ tolak atau gagal tolak H0

## Hubungan dengan Konsep Lain

- Terkait: [[P-Value]], [[Confidence Interval]], [[Type I dan Type II Error]]
- Digunakan di: [[T-Test]], [[ANOVA]], [[Chi-Square Test]], [[A-B Testing]]