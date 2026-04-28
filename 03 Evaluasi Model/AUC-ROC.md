---
tags:
  - evaluasi/klasifikasi
aliases:
  - ROC Curve
  - Area Under Curve
date: 2026-04-28
status: complete
---

# AUC-ROC

> **Ringkasan:** Area di bawah kurva ROC â€” mengukur kemampuan model membedakan kelas.

## ROC Curve

Plot **True Positive Rate** ([[Recall]]) vs **False Positive Rate** pada berbagai threshold.

## Interpretasi AUC

| AUC | Interpretasi |
|-----|-------------|
| 1.0 | Model sempurna |
| 0.5 | Model setara tebak acak |
| < 0.5 | Lebih buruk dari tebakan acak |

## Kegunaan

Membandingkan model **tanpa bergantung pada threshold tertentu**.

## Hubungan dengan Konsep Lain

- Terkait: [[Recall]], [[Specificity]], [[Confusion Matrix]], [[Log Loss]]