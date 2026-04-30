---
tags:
  - sql/ddl
aliases: []
date: 2026-04-30
status: complete
---

# TRUNCATE

> **Ringkasan:** Perintah DDL untuk menghapus semua data dalam tabel tanpa menghapus strukturnya.

## Definisi

`TRUNCATE` digunakan untuk mengosongkan isi sebuah tabel dengan cepat. Perintah ini menghapus semua baris data, namun tetap mempertahankan kerangka/struktur tabel (kolom, tipe data, index).

## Sintaks Dasar

```sql
TRUNCATE TABLE nama_tabel;
-- Contoh:
TRUNCATE TABLE mahasiswa;
```

## Karakteristik
- Lebih cepat daripada `DELETE` tanpa `WHERE`.
- Tidak bisa di-rollback pada beberapa database (tergantung transaksi).
- Mereset nilai `AUTO_INCREMENT` kembali ke awal.

## Hubungan dengan Konsep Lain

- Terkait: [[Data Definition Language]], [[DROP]], [[INSERT UPDATE DELETE]]

## Referensi
- Materi Basis Data 2024/2025 - RA
