---
tags:
  - deep-learning/arsitektur
aliases:
  - Long Short-Term Memory
date: 2026-04-28
status: complete
---

# LSTM

> **Ringkasan:** Varian [[RNN]] yang mengatasi [[Vanishing Gradient]] dengan cell state dan gates.

## Gates

| Gate | Fungsi |
|------|--------|
| **Forget gate** | Memutuskan informasi mana yang dibuang |
| **Input gate** | Memutuskan informasi baru mana yang disimpan |
| **Output gate** | Memutuskan output berdasarkan cell state |

## Hubungan dengan Konsep Lain

- Terkait: [[RNN]], [[GRU]], [[Transformer]], [[Time Series Forecasting]]