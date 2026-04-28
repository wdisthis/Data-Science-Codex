---
tags:
  - feature-engineering/cleaning
aliases:
  - Kebocoran Data
date: 2026-04-28
status: complete
---

# Data Leakage

> **Ringkasan:** Informasi dari test set bocor ke proses training â€” hasil evaluasi menjadi tidak valid.

## Contoh Umum

- Fit scaler pada seluruh data sebelum split
- Fitur yang mengandung informasi target
- Time series: menggunakan data masa depan

## Cara Mencegah

- Selalu split dulu, baru preprocess
- Gunakan [[Cross Validation|pipeline]] di [[Scikit-Learn]]
- Hati-hati dengan [[Target Encoding]]

## Hubungan dengan Konsep Lain

- Terkait: [[Train-Validation-Test Split]], [[Cross Validation]], [[Feature Engineering]]