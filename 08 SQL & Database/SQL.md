---
tags:
  - sql/dasar
aliases:
  - Structured Query Language
date: 2026-04-30
status: complete
---

# SQL

> **Ringkasan:** Bahasa standar untuk mengelola dan mengakses data dalam sistem basis data relasional (RDBMS).

## Definisi

**Structured Query Language (SQL)** adalah bahasa standar yang digunakan untuk mengelola dan mengakses data di dalam sistem basis data relasional (RDBMS) seperti MySQL, PostgreSQL, Oracle, SQL Server, dan lainnya.

SQL digunakan untuk melakukan operasi **CRUD**:
- **Create**: Membuat data baru.
- **Read**: Membaca/mengambil data.
- **Update**: Memperbarui data yang ada.
- **Delete**: Menghapus data.

## Kategori Perintah SQL

SQL dibagi menjadi beberapa kategori utama berdasarkan fungsinya:

| Kategori | Kepanjangan | Fungsi | Perintah Utama |
| :--- | :--- | :--- | :--- |
| **DDL** | [[Data Definition Language]] | Mendefinisikan struktur database | `CREATE`, `ALTER`, `DROP`, `TRUNCATE` |
| **DML** | [[Data Manipulation Language]] | Mengelola isi data dalam tabel | `INSERT`, `UPDATE`, `DELETE`, `SELECT` |
| **DCL** | Data Control Language | Mengatur hak akses dan izin | `GRANT`, `REVOKE` |
| **TCL** | Transaction Control Language | Mengelola transaksi database | `COMMIT`, `ROLLBACK`, `SAVEPOINT` |

## Hubungan dengan Konsep Lain

- Terkait: [[Data Manipulation Language]], [[Data Definition Language]]
- Digunakan di: [[PostgreSQL]], [[MySQL]], [[SQLite]]

## Referensi
- Materi Basis Data 2024/2025 - RA
