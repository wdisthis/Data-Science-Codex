---
tags:
  - feature-engineering/balancing
aliases:
  - Imbalanced Data
  - Data Tidak Seimbang
date: 2026-04-28
status: complete
---

# Class Imbalance

> **Ringkasan:** Kelas mayoritas jauh lebih banyak â†’ model cenderung mengabaikan kelas minoritas.

## Solusi

| Teknik | Deskripsi |
|--------|-----------|
| **Oversampling** | [[SMOTE]] |
| **Undersampling** | Kurangi kelas mayoritas |
| **Class Weights** | Beri bobot lebih pada minoritas |
| **Ganti metrik** | Gunakan [[F1-Score]], [[AUC-ROC]], bukan [[Accuracy]] |

## Hubungan dengan Konsep Lain

- Terkait: [[SMOTE]], [[F1-Score]], [[Cross Validation|Stratified k-Fold]]