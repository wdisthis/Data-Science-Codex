---
tags:
  - sql/ddl
aliases:
  - DDL
date: 2026-04-30
status: complete
---

# Data Definition Language

> **Ringkasan:** Kumpulan perintah SQL untuk membuat, mengubah, dan menghapus struktur objek dalam database.

## Definisi

**Data Definition Language (DDL)** adalah kumpulan perintah SQL yang digunakan untuk membuat, mengubah, dan menghapus struktur objek dalam database, seperti tabel, view, index, schema, dan lainnya. 

**Poin Penting:** DDL tidak mengelola isi data di dalam tabel, tetapi fokus pada struktur atau kerangka database itu sendiri.

## Fungsi Utama DDL

1.  Membuat objek baru (database, tabel, dll).
2.  Memodifikasi struktur objek yang sudah ada.
3.  Menghapus objek dari database.
4.  Mengatur hubungan antar tabel dan atribut.

## Perintah Utama DDL

| Perintah | Fungsi | Link Detail |
| :--- | :--- | :--- |
| **CREATE** | Membuat database atau tabel baru | [[CREATE TABLE]] |
| **ALTER** | Mengubah struktur tabel yang sudah ada | [[ALTER]] |
| **DROP** | Menghapus objek database secara permanen | [[DROP]] |
| **TRUNCATE** | Menghapus semua data dalam tabel tanpa menghapus strukturnya | [[TRUNCATE]] |
| **RENAME** | Mengganti nama tabel atau kolom | [[ALTER#4. Mengganti Nama (RENAME)]] |

## Hubungan dengan Konsep Lain

- Terkait: [[SQL]], [[Data Manipulation Language]]
- Digunakan di: [[CREATE TABLE]], [[Index Database]]

## Referensi
- Materi Basis Data 2024/2025
