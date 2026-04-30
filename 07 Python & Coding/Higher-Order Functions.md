---
tags:
  - python/konsep
aliases:
  - HOF
  - First-Class Functions
date: 2026-04-30
status: complete
---

# Higher-Order Functions

> **Ringkasan:** Fungsi yang menerima fungsi lain sebagai argumen atau mengembalikan fungsi sebagai hasil.

## First-Class Objects & Higher-Order Functions (HOF)

### First-Class Functions
Fungsi di Python adalah objek kelas utama (*first-class objects*), yang berarti fungsi bisa:
- Disimpan dalam variabel: `greet_var = greet`
- Dikirim sebagai argumen: `say_something(greet, "Alice")`
- Dikembalikan dari fungsi (Closure)
- Disimpan dalam struktur data: `list_func = [greet, say_hello]`

#### Contoh Closure
```python
def multiplier(factor):
    def multiply(x):
        return x * factor
    return multiply

double = multiplier(2)
print(double(5))  # Output: 10
```

### Higher-Order Functions (HOF)
Fungsi yang **menerima fungsi lain sebagai argumen** atau **mengembalikan fungsi**.
- **Built-in Python:** `map()`, `filter()`, `reduce()` (`functools`), `sorted(key=...)`
- **Konteks JS:** Sering disebut sebagai pola *callback*.

## Hubungan dengan Konsep Lain
- [[Functional Programming]]
- [[Lambda Function]]
- [[Decorator]]
