---
tags:
  - sql/ddl
aliases: []
date: 2026-04-30
status: complete
---

# DROP

> **Ringkasan:** Perintah DDL untuk menghapus objek database secara permanen.

## Definisi

Perintah `DROP` digunakan untuk menghapus objek database seperti tabel, database, view, atau index. **Peringatan:** Tindakan ini bersifat permanen dan akan menghapus seluruh struktur serta data yang ada di dalamnya.

## Sintaks Dasar

### Menghapus Tabel
```sql
DROP TABLE nama_tabel;
-- Contoh:
DROP TABLE mahasiswa;
```

### Menghapus Database
```sql
DROP DATABASE nama_database;
-- Contoh:
DROP DATABASE perpustakaan;
```

## Perbedaan dengan TRUNCATE
Berbeda dengan [[TRUNCATE]], `DROP` menghapus **struktur** objeknya juga, bukan hanya isinya.

## Hubungan dengan Konsep Lain

- Terkait: [[Data Definition Language]], [[TRUNCATE]]

## Referensi
- Materi Basis Data 2024/2025 - RA
