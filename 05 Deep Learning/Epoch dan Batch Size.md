---
tags:
  - deep-learning/fondasi
  - terminologi
aliases:
  - Epoch
  - Batch Size
  - Iteration
date: 2026-04-28
status: complete
---

# Epoch dan Batch Size

> **Ringkasan:** Parameter training yang mengatur bagaimana data diproses selama training.

## Definisi

| Istilah | Definisi |
|---------|----------|
| **Epoch** | Satu kali pass lengkap seluruh data training |
| **Batch Size** | Jumlah sampel diproses sebelum update bobot |
| **Iteration** | Satu kali update bobot (= total_data / batch_size per epoch) |

## Tips

- Batch size kecil â†’ lebih noisy tapi generalisasi lebih baik
- Batch size besar â†’ training lebih stabil tapi butuh lebih banyak memory

## Hubungan dengan Konsep Lain

- Terkait: [[Gradient Descent]], [[Neural Network]], [[Learning Rate]]