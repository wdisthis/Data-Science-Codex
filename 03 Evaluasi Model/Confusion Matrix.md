---
tags:
  - evaluasi/klasifikasi
date: 2026-04-28
status: complete
---

# Confusion Matrix

> **Ringkasan:** Tabel yang merangkum performa model klasifikasi.

## Struktur

```
                  Predicted
                  Pos    Neg
Actual  Pos  |  TP   |  FN  |
        Neg  |  FP   |  TN  |
```

- **TP (True Positive):** Prediksi positif, aktual positif
- **TN (True Negative):** Prediksi negatif, aktual negatif
- **FP (False Positive):** Prediksi positif, aktual negatif â†’ [[Type I dan Type II Error|Type I]]
- **FN (False Negative):** Prediksi negatif, aktual positif â†’ [[Type I dan Type II Error|Type II]]

## Metrik Turunan

- [[Accuracy]], [[Precision]], [[Recall]], [[F1-Score]], [[Specificity]]

## Hubungan dengan Konsep Lain

- Terkait: [[AUC-ROC]], [[Type I dan Type II Error]]
- Visualisasi: [[Heatmap]]
- Library: [[Scikit-Learn]]