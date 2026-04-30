---
tags:
  - python/dasar
aliases:
  - arguments
  - keyword arguments
date: 2026-04-30
status: complete
---

# Args and Kwargs

> **Ringkasan:** `*args` dan `**kwargs` digunakan untuk menangani argumen dalam jumlah yang fleksibel pada fungsi Python.

## Penanganan Argumen: `*args` & `**kwargs`
Sebelum memahami dekorator, penting mengetahui cara fungsi menerima argumen secara fleksibel.

| Tipe | Deskripsi | Struktur Data | Contoh |
|------|-----------|---------------|--------|
| **Fixed Parameters** | Jumlah argumen sudah ditentukan & tetap | - | `def func(a, b, c):` |
| **`*args`** | Menerima **argumen posisi** berjumlah tak terbatas | `tuple` | `def sum_all(*numbers):` |
| **`**kwargs`** | Menerima **argumen kunci (key-value)** | `dictionary` | `def print_data(**kwargs):` |

### Contoh Kode
```python
# *args
def sum_all(*numbers):
    return sum(numbers)
print(sum_all(2, 3, 4, 5))  # Output: 14

# **kwargs
def print_data(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
print_data(nama="Budi", umur=20)
# Output:
# nama: Budi
# umur: 20
```

## Hubungan dengan Konsep Lain
- [[Python Basics]]
- [[Decorator]]
