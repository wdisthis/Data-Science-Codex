---
tags:
  - sql/ddl
aliases:
  - ALTER TABLE
  - RENAME
date: 2026-04-30
status: complete
---

# ALTER

> **Ringkasan:** Perintah DDL untuk mengubah struktur tabel yang sudah ada.

## Definisi

Perintah `ALTER` digunakan ketika kita perlu memodifikasi kerangka tabel tanpa harus menghapus dan membuatnya kembali.

## Operasi Utama

### 1. Menambah Kolom Baru (ADD)
Digunakan untuk menambahkan atribut baru ke tabel.
```sql
ALTER TABLE nama_tabel ADD nama_kolom tipe_data;
-- Contoh:
ALTER TABLE mahasiswa ADD email VARCHAR(100);
```

### 2. Mengubah Tipe Data Kolom (MODIFY)
Digunakan untuk mengubah jenis data atau panjang karakter kolom.
```sql
ALTER TABLE nama_tabel MODIFY nama_kolom tipe_data;
-- Contoh:
ALTER TABLE mahasiswa MODIFY email VARCHAR(150);
```

### 3. Menghapus Kolom (DROP COLUMN)
Digunakan untuk menghilangkan kolom yang tidak diperlukan lagi.
```sql
ALTER TABLE nama_tabel DROP COLUMN nama_kolom;
-- Contoh:
ALTER TABLE mahasiswa DROP COLUMN email;
```

### 4. Mengganti Nama (RENAME)
Digunakan untuk mengganti nama tabel atau nama kolom.
```sql
-- Mengganti nama tabel
ALTER TABLE nama_tabel RENAME TO nama_tabel_baru;
-- Contoh:
ALTER TABLE mahasiswa RENAME TO siswa;
```

## Contoh Praktis (Studi Kasus Rental Mobil)

### Menambah kolom tahun kendaraan
```sql
ALTER TABLE kendaraan ADD tahun_kendaraan DATE;
```

### Mengubah tipe data tahun kendaraan
```sql
ALTER TABLE kendaraan MODIFY tahun_kendaraan YEAR;
```

### Mengganti nama tabel transaksi menjadi sewa
```sql
ALTER TABLE transaksi RENAME TO sewa;
```

## Hubungan dengan Konsep Lain

- Terkait: [[Data Definition Language]], [[CREATE TABLE]]
- Digunakan di: [[Index Database]]

## Referensi
- Materi Basis Data 2024/2025 - RA
