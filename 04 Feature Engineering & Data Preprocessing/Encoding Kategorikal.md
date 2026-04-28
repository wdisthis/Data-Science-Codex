---
tags:
  - feature-engineering/encoding
aliases:
  - Categorical Encoding
date: 2026-04-28
status: complete
---

# Encoding Kategorikal

> **Ringkasan:** Mengubah data kategorikal menjadi numerik agar bisa diproses model ML.

## Teknik

| Teknik | Kapan Digunakan |
|--------|-----------------|
| [[One-Hot Encoding]] | Kategori nominal, jumlah sedikit |
| [[Label Encoding]] | Kategori ordinal (ada urutan) |
| [[Target Encoding]] | High cardinality |
| Binary Encoding | Kompromi one-hot dan label |

## Hubungan dengan Konsep Lain

- Terkait: [[Feature Engineering]], [[Pandas]], [[Scikit-Learn]]