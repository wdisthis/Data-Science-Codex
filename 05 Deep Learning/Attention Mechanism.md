---
tags:
  - deep-learning/arsitektur
aliases:
  - Self-Attention
  - Multi-Head Attention
date: 2026-04-28
status: complete
---

# Attention Mechanism

> **Ringkasan:** Memungkinkan model fokus pada bagian input yang paling relevan.

## Tipe

- **Self-Attention:** Setiap token memperhatikan semua token lain dalam sekuens
- **Cross-Attention:** Satu sekuens memperhatikan sekuens lain
- **Multi-Head Attention:** Beberapa attention heads paralel

## Query, Key, Value

`Attention(Q, K, V) = softmax(QK^T / sqrt(dk)) * V`

## Hubungan dengan Konsep Lain

- Terkait: [[Transformer]], [[BERT]], [[GPT]]