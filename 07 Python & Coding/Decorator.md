---
tags:
  - python/dasar
aliases:
  - dekorator
date: 2026-04-30
status: complete
---

# Decorator

> **Ringkasan:** Decorator adalah fungsi yang memodifikasi perilaku fungsi lain tanpa mengubah kode aslinya.

## Konsep & Struktur

### Definisi
Decorator adalah fungsi yang:
1. Menerima fungsi lain sebagai argumen.
2. Menambahkan perilaku/fitur baru.
3. Mengembalikan fungsi yang telah dimodifikasi **tanpa mengubah kode asli**.

### Sintaks & Prinsip
- Ditandai dengan simbol `@` tepat di atas deklarasi fungsi.
- Menerapkan prinsip **DRY** (*Don't Repeat Yourself*): memisahkan logika tambahan (validasi, logging, dll) dari logika utama.
- **Alur Eksekusi:** `FUNGSI ASLI → DECORATOR → FUNGSI TERDEKORASI`

### Struktur Dasar
```python
def my_decorator(func):
    def wrapper():
        print("Sebelum fungsi dijalankan.")
        func()
        print("Setelah fungsi dijalankan.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
# Output:
# Sebelum fungsi dijalankan.
# Hello!
# Setelah fungsi dijalankan.
```

---

## Tujuan & Implementasi Dekorator

| Tujuan | Penjelasan | Contoh Implementasi |
|--------|------------|---------------------|
| **Validasi Input** | Cek kriteria sebelum eksekusi (hindari error) | `validate_nonzero` (cegah pembagian nol) |
| **Transformasi Data** | Ubah format hasil keluaran fungsi | `uppercase_decorator` (ubah ke huruf besar) |
| **Logging / Debug** | Catat argumen masuk & hasil keluar untuk tracking | `debug_decorator` |
| **Open/Closed Principle** | Tambah fitur tanpa mengubah fungsi asli | Semua contoh di atas |
| **Maintenance** | Logika tambahan terpusat di 1 tempat | Mudah diubah/dihapus tanpa sentuh core logic |

### Contoh 1: Validasi (Cegah Error)
```python
def validate_nonzero(func):
    def wrapper(a, b):
        if b == 0:
            return "Tidak bisa dibagi dengan nol!"
        return func(a, b)
    return wrapper

@validate_nonzero
def bagi(a, b):
    return a / b

print(bagi(10, 2))  # 5.0
print(bagi(10, 0))  # Tidak bisa dibagi dengan nol!
```

### Contoh 2: Transformasi & Logging
```python
def uppercase_decorator(func):
    def wrapper(*args, **kwargs):
        result = func(*args, **kwargs)
        return result.upper()
    return wrapper

def debug_decorator(func):
    def wrapper(*args, **kwargs):
        print(f"[DEBUG] Args: {args}, Kwargs: {kwargs}")
        return func(*args, **kwargs)
    return wrapper
```

---

## Latihan Soal & Penyelesaian

**Soal:**  
Buatlah decorator `log_decorator` yang mencetak pesan sebelum dan sesudah fungsi `hello(name)` dipanggil.

**Jawaban:**
```python
def log_decorator(func):
    def wrapper(*args, **kwargs):
        print("Memulai fungsi...")
        result = func(*args, **kwargs)
        print("Fungsi selesai.")
        return result
    return wrapper

@log_decorator
def hello(name):
    print(f"Hello, {name}")

hello("Budi")
```
**Output:**
```
Memulai fungsi...
Hello, Budi
Fungsi selesai.
```

---

## 💡 Best Practice: `functools.wraps`
Saat membuat decorator, disarankan menggunakan `@functools.wraps(func)` pada fungsi `wrapper` agar **metadata fungsi asli** (seperti `__name__`, `__doc__`) tidak hilang:
```python
import functools

def log_decorator(func):
    @functools.wraps(func)
    def wrapper(*args, **kwargs):
        print("Memulai fungsi...")
        return func(*args, **kwargs)
    return wrapper
```

## Hubungan dengan Konsep Lain
- [[Args and Kwargs]]
- [[Higher-Order Functions]]
- [[Functional Programming]]