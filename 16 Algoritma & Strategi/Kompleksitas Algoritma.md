---
tags:
  - algoritma
  - matematika
aliases:
  - Big O Notation
  - Efisiensi Algoritma
date: 2026-05-01
status: complete
---

# Kompleksitas Algoritma

> **Ringkasan:** Pengukuran efisiensi sebuah algoritma dalam hal penggunaan waktu (eksekusi) dan ruang (memori) relatif terhadap ukuran masukan.

## 1. Definisi
Sebuah algoritma tidak hanya harus benar secara logika, tetapi juga harus **mangkus (efisien)**. Algoritma yang benar tetapi memakan waktu bertahun-tahun untuk berjalan seringkali tidak berguna dalam prakteknya.

## 2. Jenis Kompleksitas
Kompleksitas diukur sebagai fungsi dari ukuran masukan ($n$):

### A. Kompleksitas Waktu ($T(n)$)
Mengukur jumlah tahapan komputasi atau "langkah" yang dilakukan oleh algoritma.
* **Operasi Dasar**: Dalam analisis, kita fokus pada operasi khas yang paling sering dilakukan (misal: perbandingan dalam sorting, perkalian dalam matriks).
* **Worst Case ($O$ / Big O)**: Batas atas waktu eksekusi (skenario terburuk).
* **Best Case ($\Omega$)**: Batas bawah waktu eksekusi.
* **Average Case ($\Theta$)**: Ekspektasi waktu eksekusi rata-rata.

### B. Kompleksitas Ruang ($S(n)$)
Mengukur jumlah memori (RAM) yang dibutuhkan oleh algoritma selama eksekusi. Ini mencakup variabel, struktur data, dan *stack* rekursif.

---

## 3. Notasi Big O (Order of Growth)
Urutan kompleksitas dari yang paling efisien ke yang paling lambat:
1. $O(1)$ - Konstan
2. $O(\log n)$ - Logaritmik (Contoh: Binary Search)
3. $O(n)$ - Linear (Contoh: Linear Search)
4. $O(n \log n)$ - Linearithmic (Contoh: Merge Sort)
5. $O(n^2)$ - Kuadratik (Contoh: Bubble Sort)
6. $O(2^n)$ - Eksponensial (Contoh: Solusi Naif TSP)
7. $O(n!)$ - Faktorial

---

## 4. Pentingnya Analisis
Analisis kompleksitas membantu kita:
* Membandingkan dua algoritma untuk masalah yang sama.
* Memprediksi waktu eksekusi saat ukuran data meningkat (skalabilitas).
* Mengidentifikasi *bottleneck* dalam sistem.

## Hubungan dengan Konsep Lain
- Terkait: [[Strategi Algoritma]], [[Searching & Sorting]]
