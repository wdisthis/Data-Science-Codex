---
tags:
  - evaluasi/klasifikasi
aliases:
  - Akurasi
date: 2026-04-28
status: complete
---

# Accuracy

> **Ringkasan:** Proporsi prediksi yang benar dari total prediksi.

## Rumus

`Accuracy = (TP + TN) / Total`
$$Accuracy = \frac{TP + TN}{TP + TN + FP + FN}$$

## Kapan Digunakan

Data **seimbang**. Jangan gunakan saat [[Class Imbalance]] â€” gunakan [[F1-Score]] atau [[AUC-ROC]].

## Hubungan dengan Konsep Lain

- Terkait: [[Confusion Matrix]], [[Precision]], [[Recall]]