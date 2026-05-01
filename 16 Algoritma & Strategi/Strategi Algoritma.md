---
tags:
  - algoritma
  - konsep
aliases:
  - Algorithm Strategies
  - Klasifikasi Algoritma
date: 2026-05-01
status: complete
---

# Strategi Algoritma

> **Ringkasan:** Pendekatan umum untuk memecahkan persoalan secara algoritmis yang dapat diterapkan pada berbagai bidang komputasi. Strategi ini membantu dalam merancang solusi yang efisien dan terstruktur.

## 1. Definisi dan Alasan Mempelajari Strategi Algoritma
* **Definisi**: Strategi algoritma adalah pendekatan umum atau "blueprint" untuk memecahkan masalah. Ia bukan sekadar kode, melainkan logika di balik bagaimana solusi ditemukan.
* **Tujuan**:
    1. Memberikan panduan dalam merancang algoritma untuk persoalan baru.
    2. Membantu mengklasifikasikan algoritma berdasarkan gagasan perancangannya.
    3. Memfasilitasi analisis kinerja dan efisiensi sejak tahap desain.

---

## 2. Klasifikasi Strategi Algoritma
Strategi algoritma diklasifikasikan ke dalam beberapa pendekatan utama:

### A. Strategi Solusi Langsung (Direct Solution)
* **[[Brute Force]]**: Pendekatan lempang (straightforward) yang mencoba semua kemungkinan untuk menemukan solusi. Biasanya lambat tetapi dijamin benar.
* **[[Greedy Algorithm]]**: Memilih opsi terbaik yang tersedia di setiap langkah (local optimum) dengan harapan menemukan solusi terbaik secara keseluruhan (global optimum).

### B. Strategi Berbasis Pencarian Ruang Status
* **[[Backtracking]]**: Mencari solusi dengan menelusuri pohon ruang status secara DFS. Jika langkah tidak menuju solusi, algoritma akan "mundur" (backtrack).
* **Branch and Bound**: Mirip dengan backtracking, tetapi menggunakan teknik pemangkasan (pruning) untuk mengabaikan cabang yang tidak mungkin menghasilkan solusi optimal.

![Pohon Ruang Status](C:\Users\LENOVO\.gemini\antigravity\brain\3a6d2988-e0b9-49a2-8c04-3015d50519a8\state_space_tree_1777649446693.png)

### C. Strategi Atas-Bawah (Top-Down)
* **[[Divide and Conquer]]**: Membagi persoalan menjadi sub-persoalan yang lebih kecil, menyelesaikannya secara independen, lalu menggabungkan hasilnya.

### D. Strategi Bawah-Atas (Bottom-Up)
* **[[Dynamic Programming]]**: Menyelesaikan persoalan dengan memecahnya menjadi sub-persoalan yang tumpang tindih (overlapping) dan menyimpan hasil sub-persoalan tersebut (memoization) agar tidak dihitung ulang.

---

## 3. Contoh Persoalan Klasik
Berikut adalah beberapa persoalan terkenal yang sering digunakan sebagai studi kasus strategi algoritma:

| Nama Persoalan | Deskripsi Singkat | Strategi Umum |
| :--- | :--- | :--- |
| **TSP** (*Traveling Salesperson*) | Mencari jalur terpendek melalui sejumlah kota dan kembali ke kota asal. | Brute Force, Dynamic Programming, Greedy |
| **Knapsack Problem** | Memilih objek dengan bobot tertentu untuk keuntungan maksimal tanpa melebihi kapasitas. | Greedy, Dynamic Programming, Branch & Bound |
| **Assignment Problem** | Menugaskan $n$ orang ke $n$ pekerjaan dengan total biaya seminimal mungkin. | Brute Force, Branch & Bound |
| **N-Queens Problem** | Menempatkan $N$ ratu di papan catur $N \times N$ tanpa saling menyerang. | Backtracking |
| **Graph Colouring** | Mewarnai simpul graf sehingga tidak ada tetangga yang sewarna. | Backtracking, Greedy |
| **Maze Problem** | Menemukan jalan keluar dari sebuah labirin. | Backtracking, BFS/DFS |

---

## 4. Pokok Bahasan Lanjutan
* **Decrease and Conquer**: Reduksi ukuran persoalan di setiap langkah (misal: Binary Search).
* **Graph Search**: [[Tree Traversal]] menggunakan **Breadth-First Search (BFS)** dan **Depth-First Search (DFS)**.
* **Pencarian Heuristik**: Algoritma cerdas seperti **$A^*$**, **Best First Search**, dan **UCS** (Uniform Cost Search).
* **Pencocokan String**: Teknik *String Matching* dan *Regular Expression* (Regex) untuk pencarian pola teks.

## Hubungan dengan Konsep Lain
- Lanjut ke: [[Kompleksitas Algoritma]]
- Terkait: [[_MOC Algoritma]], [[Recursive Algorithm]]
