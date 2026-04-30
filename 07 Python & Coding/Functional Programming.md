---
tags:
  - python/konsep
  - programming/paradigm
aliases:
  - Paradigma Fungsional
date: 2026-04-30
status: complete
---

# Functional Programming

> **Ringkasan:** Paradigma pemrograman yang berfokus pada penggunaan fungsi murni dan data yang tidak berubah (immutable).

## Prinsip Dasar Functional Programming
Dekorator dibangun di atas prinsip-prinsip berikut:
1. **Pure Functions** → Input sama selalu menghasilkan output sama, tanpa *side effects*.
2. **Immutability** → Data tidak dimodifikasi langsung; buat salinan/versi baru jika perlu perubahan.
3. **First-Class Functions** → Fungsi diperlakukan sebagai objek/data biasa.
4. **Declarative Style** → Fokus pada *"apa"* yang dilakukan (pakai `map`, `filter`, `reduce`), bukan *"bagaimana"* (loop manual).
5. **Recursion** → Mengganti perulangan dengan pemanggilan fungsi secara mandiri.

## Hubungan dengan Konsep Lain
- [[Lambda Function]]
- [[Higher-Order Functions]]
- [[Decorator]]
