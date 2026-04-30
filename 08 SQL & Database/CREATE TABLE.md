---
tags:
  - sql/ddl
aliases: []
date: 2026-04-30
status: complete
---

# CREATE TABLE

> **Ringkasan:** Perintah DDL untuk membuat tabel baru di dalam database.

## Definisi

Perintah `CREATE` digunakan untuk membuat objek database baru. Dalam konteks tabel, ia mendefinisikan nama tabel, nama kolom, tipe data, dan batasan (constraint).

## Sintaks Dasar

### Membuat Database
```sql
CREATE DATABASE nama_database;
-- Contoh:
CREATE DATABASE siakad;
```

### Membuat Tabel
```sql
CREATE TABLE nama_tabel (
    nama_kolom1 tipe_data [CONSTRAINT],
    nama_kolom2 tipe_data [CONSTRAINT],
    ...
);
```

## Contoh Praktis

### Membuat Tabel Mahasiswa
```sql
CREATE TABLE mahasiswa (
    id_mahasiswa INT PRIMARY KEY,
    nama VARCHAR(100),
    jurusan VARCHAR(50),
    angkatan YEAR
);
```

### Studi Kasus: Rental Mobil
```sql
-- 1. Buat database
CREATE DATABASE rental;

-- 2. Buat tabel pelanggan
CREATE TABLE pelanggan (
    no_ktp INT(16) PRIMARY KEY,
    nama_lengkap VARCHAR(30),
    alamat TEXT,
    no_rekening INT(20)
);

-- 3. Buat tabel kendaraan
CREATE TABLE kendaraan (
    no_bpkb INT(14) PRIMARY KEY,
    jenis_kendaraan VARCHAR(15),
    kondisi TEXT
);

-- 4. Buat tabel transaksi (dengan Foreign Key)
CREATE TABLE transaksi (
    id_transaksi INT(14) PRIMARY KEY AUTO_INCREMENT,
    no_ktp INT,
    no_bpkb INT,
    tanggal_peminjaman DATE,
    tanggal_pengembalian DATE,
    FOREIGN KEY (no_ktp) REFERENCES pelanggan (no_ktp),
    FOREIGN KEY (no_bpkb) REFERENCES kendaraan (no_bpkb)
);
```

## Hubungan dengan Konsep Lain

- Terkait: [[Data Definition Language]], [[Primary Key dan Foreign Key]]
- Digunakan di: [[Normalisasi Database]]

## Referensi
- Materi Basis Data 2024/2025 - RA