---
tags:
  - sql/dml
aliases:
  - DML
date: 2026-04-30
status: complete
---

# INSERT UPDATE DELETE

> **Ringkasan:** Perintah DML untuk memanipulasi data di dalam tabel.

## INSERT
Digunakan untuk menambahkan baris data baru ke dalam tabel.
```sql
INSERT INTO nama_tabel (kolom1, kolom2) VALUES (nilai1, nilai2);
-- Contoh:
INSERT INTO mahasiswa (id_mahasiswa, nama) VALUES (1, 'Budi');
```

## UPDATE
Digunakan untuk memperbarui data yang sudah ada di dalam tabel.
```sql
UPDATE nama_tabel SET kolom1 = nilai_baru WHERE kondisi;
-- Contoh:
UPDATE mahasiswa SET nama = 'Budi Santoso' WHERE id_mahasiswa = 1;
```

## DELETE
Digunakan untuk menghapus baris data dari tabel.
```sql
DELETE FROM nama_tabel WHERE kondisi;
-- Contoh:
DELETE FROM mahasiswa WHERE id_mahasiswa = 1;
```

## Hubungan dengan Konsep Lain
- Terkait: [[SELECT]], [[Data Manipulation Language]], [[Transaction]]
- Digunakan di: [[CRISP-DM]]

## Referensi
- Materi Basis Data 2024/2025