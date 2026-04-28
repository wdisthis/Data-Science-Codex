---
tags:
  - deep-learning/arsitektur
aliases:
  - Transformer Architecture
date: 2026-04-28
status: complete
---

# Transformer

> **Ringkasan:** Arsitektur revolusioner berbasis [[Attention Mechanism]] â€” dasar model bahasa modern.

## Komponen Utama

- **Encoder:** Memproses input (digunakan di [[BERT]])
- **Decoder:** Menghasilkan output (digunakan di [[GPT]])
- **Self-Attention:** Setiap token memperhatikan semua token lain

## Keunggulan vs RNN

- Paralelisasi penuh (tidak sequential)
- Lebih baik menangkap long-range dependencies

## Hubungan dengan Konsep Lain

- Terkait: [[Attention Mechanism]], [[BERT]], [[GPT]], [[LLM]]
- Dibandingkan: [[RNN]], [[LSTM]]