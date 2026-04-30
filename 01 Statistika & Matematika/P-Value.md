---
tags:
  - statistik/inferensial
aliases:
  - nilai-p
  - p value
date: 2026-04-29
status: complete
Audithor: Fitra
---

# P-Value

> **Ringkasan:** Probabilitas mendapatkan hasil yang sama ekstrem (atau lebih ekstrem) dengan data yang diamati, *jika hipotesis nol (H0) benar*.

## Definisi

P-value mengukur seberapa konsisten data yang diamati dengan [[Hipotesis]] nol. Semakin kecil p-value, semakin kuat bukti melawan H0.

## Interpretasi

- `p < 0.05` → Tolak H0 (hasil dianggap signifikan secara statistik)
- `p >= 0.05` → Gagal tolak H0 (tidak cukup bukti melawan H0)

> [!WARNING]
> p-value **BUKAN** probabilitas bahwa H0 benar. Signifikansi statistik ≠ signifikansi praktis.

## Contoh
Uji apakah rata-rata tinggi badan pria dan wanita berbeda → p = 0.02 → ada perbedaan signifikan.

## Level Signifikansi ($\alpha$)
P-value tidak berdiri sendiri. Ia selalu dibandingkan dengan **$\alpha$** (Alpha), yaitu ambang batas risiko yang siap Anda tanggung untuk melakukan _Type I Error_ (menolak $H_0$ padahal benar).

Umumnya $\alpha = 0.05$, tapi dalam bidang medis atau teknik yang sangat presisi, $\alpha$ bisa diset jauh lebih rendah (misal $0.01$ atau $0.001$).

## P-value vs. Efek Ukuran (_Effect Size_)
Seperti yang tercatat pada poin signifikansi praktis, p-value sangat sensitif terhadap **ukuran sampel**.

- **Sampel Besar:** Perbedaan yang sangat kecil (tidak penting secara nyata) bisa menghasilkan p-value $< 0.05$ hanya karena jumlah datanya banyak.
- **Sampel Kecil:** Perbedaan yang besar dan nyata secara praktis mungkin menghasilkan p-value $> 0.05$ karena kurangnya kekuatan statistik (_power_).

### Visualisasi

Dalam distribusi normal (atau distribusi $t$), p-value adalah **luas area di bawah kurva** pada bagian ekor (_tail_) yang dimulai dari titik nilai statistik hitung Anda. Semakin jauh statistik hitung dari pusat (rata-rata), semakin kecil luas areanya, sehingga semakin kecil pula p-value-nya.
## Hubungan dengan Konsep Lain

- Terkait: [[Hipotesis]], [[Confidence Interval]], [[Type I dan Type II Error]]
- Digunakan di: [[T-Test]], [[ANOVA]], [[Chi-Square Test]], [[A-B Testing]]
- Library: [[Statsmodels]], [[SciPy]]