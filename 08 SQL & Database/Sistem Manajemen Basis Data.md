---
tags:
  - sql/database
  - konsep
aliases:
  - DBMS
  - Database Management System
date: 2026-05-01
status: complete
---

# Sistem Manajemen Basis Data

> **Ringkasan:** Dasar-dasar sistem basis data, perbedaan antara data dan informasi, serta keuntungan menggunakan DBMS dibandingkan sistem file tradisional.

## 1. Konsep Dasar Data dan Informasi
* **Data**: Fakta-fakta mengenai objek atau orang yang dapat disimpan dan memiliki arti tertentu. Data dinyatakan dalam bentuk angka, deretan karakter, atau simbol.
* **Komponen Data**:
    * **Elemen Data**: Satuan data terkecil yang tidak dapat dipecah lagi.
    * **Rekaman (Record)**: Gabungan elemen data yang saling berhubungan.
    * **Berkas (File)**: Kumpulan record bertipe sama, seperti data mahasiswa atau dosen.
* **Informasi**: Hasil pengolahan data yang digunakan sebagai acuan dalam pengambilan keputusan.

---

## 2. Basis Data dan Sistem Basis Data
* **Basis Data**: Representasi fakta dunia nyata (objek) yang direkam dalam bentuk teks, angka, gambar, atau bunyi. Secara harfiah berarti gudang atau tempat berkumpul.
* **Sistem**: Tatanan komponen fungsional yang saling berhubungan untuk memenuhi pekerjaan tertentu.
* **Komponen Sistem Basis Data**:
    * **Hardware**: Komputer, media penyimpan, dan perangkat jaringan.
    * **Operating System**: Perangkat lunak untuk mengendalikan sumber daya komputer.
    * **Database**: Basis data yang mewakili sistem tertentu.
    * **DBMS (Database Management System)**: Perangkat lunak pengelola basis data (Contoh: MS. Access, Oracle, SQL Server).
    * **User**: Orang yang merancang atau menggunakan sistem.

![Arsitektur DBMS](C:\Users\LENOVO\.gemini\antigravity\brain\3a6d2988-e0b9-49a2-8c04-3015d50519a8\dbms_architecture_1777648983887.png)

---

## 3. Keuntungan Model Terintegrasi (DBMS) vs Sistem File
* **Kelemahan Sistem File**: Terjadi pengulangan data (redundansi), inkonsistensi, kesulitan akses, dan masalah keamanan.
* **Keuntungan DBMS**:
    * Mengurangi perulangan data.
    * Mencapai independensi data.
    * Integrasi data dari berbagai file.
    * Kecepatan akses informasi dan peningkatan keamanan.

## Hubungan dengan Konsep Lain
- Terkait: [[SQL]], [[Normalisasi Database]]
- Lanjut ke: [[Siklus Hidup Perancangan Basis Data]]
