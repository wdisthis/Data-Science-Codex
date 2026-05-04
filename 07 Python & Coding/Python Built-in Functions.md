---
tags:
  - python/dasar
  - documentation
aliases:
  - Built-in Functions
date: 2026-05-04
status: complete
---

# 🛠️ Python Built-in Functions

> **Ringkasan:** Python menyediakan 71 fungsi bawaan (built-in) yang selalu tersedia tanpa perlu melakukan import modul tambahan. Fungsi-fungsi ini adalah fondasi utama dari bahasa pemrograman Python.

---

## 🔢 1. Matematika & Tipe Numerik
Fungsi untuk operasi matematika dasar dan konversi tipe data angka.

| Fungsi          | Deskripsi                                           | Contoh                     |
| :-------------- | :-------------------------------------------------- | :------------------------- |
| `abs(x)`        | Mengembalikan nilai absolut dari sebuah angka.      | `abs(-5)` → `5`            |
| `bool(x)`       | Mengonversi nilai menjadi Boolean (`True`/`False`). | `bool(0)` → `False`        |
| `complex(r, i)` | Membuat angka kompleks.                             | `complex(2, 3)` → `(2+3j)` |
| `divmod(a, b)`  | Mengembalikan (kuosien, sisa pembagian).            | `divmod(10, 3)` → `(3, 1)` |
| `float(x)`      | Mengonversi angka/string menjadi float.             | `float("3.14")` → `3.14`   |
| `int(x)`        | Mengonversi angka/string menjadi integer.           | `int(3.9)` → `3`           |
| `max(...)`      | Mengambil nilai terbesar.                           | `max(1, 5, 2)` → `5`       |
| `min(...)`      | Mengambil nilai terkecil.                           | `min(1, 5, 2)` → `1`       |
| `pow(x, y, z)`  | Menghitung $x^y$ (opsional: modulo $z$).            | `pow(2, 3)` → `8`          |
| `round(x, n)`   | Membulatkan angka ke $n$ desimal.                   | `round(3.456, 2)` → `3.46` |
| `sum(iterable)` | Menjumlahkan seluruh elemen dalam iterable.         | `sum([1, 2, 3])` → `6`     |

---

## 📚 2. Koleksi & Urutan (Collections)
Fungsi untuk membuat dan mengelola struktur data seperti list, dict, dan set.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `dict(...)` | Membuat dictionary baru. | `dict(a=1, b=2)` |
| `enumerate(it)` | Menambahkan index pada elemen iterable. | `list(enumerate(['a', 'b']))` → `[(0, 'a'), (1, 'b')]` |
| `frozenset(it)`| Membuat set yang tidak bisa diubah (immutable). | `frozenset([1, 2])` |
| `len(s)` | Mengembalikan panjang (jumlah item) objek. | `len("halo")` → `4` |
| `list(it)` | Membuat list dari iterable. | `list((1, 2))` → `[1, 2]` |
| `range(...)` | Membuat deret angka (lazy evaluation). | `list(range(3))` → `[0, 1, 2]` |
| `reversed(seq)` | Membalikkan urutan elemen. | `list(reversed([1, 2]))` → `[2, 1]` |
| `set(it)` | Membuat set baru (unik). | `set([1, 1, 2])` → `{1, 2}` |
| `slice(...)` | Membuat objek slice untuk pemotongan urutan. | `s = slice(1, 3); [0,1,2,3][s]` → `[1, 2]` |
| `sorted(it)` | Mengembalikan list baru yang terurut. | `sorted([3, 1, 2])` → `[1, 2, 3]` |
| `tuple(it)` | Membuat tuple baru. | `tuple([1, 2])` → `(1, 2)` |

---

## 🔤 3. String, Bytes & Karakter
Fungsi untuk manipulasi teks dan representasi biner.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `ascii(obj)` | Representasi string dengan escape karakter non-ASCII. | `ascii("ñ")` → `'\\xf1'` |
| `bin(x)` | Mengonversi integer ke string biner. | `bin(3)` → `'0b11'` |
| `bytearray()` | Membuat array byte yang bisa diubah (mutable). | `bytearray(5)` |
| `bytes()` | Membuat objek byte (immutable). | `bytes([65, 66])` → `b'AB'` |
| `chr(i)` | Mengonversi kode Unicode ke karakter. | `chr(97)` → `'a'` |
| `format(v, f)` | Memformat nilai berdasarkan spesifikasi. | `format(0.5, '%')` → `'50.000000%'` |
| `hex(x)` | Mengonversi integer ke string heksadesimal. | `hex(255)` → `'0xff'` |
| `oct(x)` | Mengonversi integer ke string oktal. | `oct(8)` → `'0o10'` |
| `ord(c)` | Mengonversi karakter ke kode Unicode (integer). | `ord('a')` → `97` |
| `repr(obj)` | Mengembalikan representasi string "printable". | `repr("a")` → `"'a'"` |
| `str(obj)` | Mengonversi objek menjadi string. | `str(10)` → `'10'` |

---

## ⚙️ 4. Iterasi & Pemrograman Fungsional
Alat untuk memproses data secara deklaratif.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `all(it)` | `True` jika **semua** elemen bersifat truthy. | `all([True, 1, ""])` → `False` |
| `any(it)` | `True` jika **ada salah satu** elemen truthy. | `any([False, 0, 1])` → `True` |
| `filter(fn, it)`| Menyaring elemen berdasarkan fungsi. | `filter(lambda x: x>0, [-1, 1])` |
| `iter(obj)` | Mengembalikan objek iterator. | `it = iter([1, 2])` |
| `map(fn, it)` | Menerapkan fungsi ke setiap elemen. | `map(str.upper, ['a', 'b'])` |
| `next(it)` | Mengambil elemen berikutnya dari iterator. | `next(it)` |
| `zip(*its)` | Menggabungkan beberapa iterable secara paralel. | `zip([1,2], ['a','b'])` |

---

## 🔍 5. Introspeksi & Objek
Fungsi untuk memeriksa properti dan identitas objek.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `callable(obj)` | Memeriksa apakah objek bisa dipanggil (fungsi/class).| `callable(print)` → `True` |
| `dir(obj)` | List atribut dan metode dari sebuah objek. | `dir([])` |
| `hasattr(o, n)` | Memeriksa apakah objek memiliki atribut tertentu. | `hasattr(str, "upper")` → `True` |
| `id(obj)` | Mengembalikan ID unik (alamat memori) objek. | `id(x)` |
| `isinstance(o, c)`| Memeriksa apakah objek adalah instance dari class. | `isinstance(5, int)` → `True` |
| `issubclass(d, p)`| Memeriksa hubungan inheritance antar class. | `issubclass(bool, int)` → `True` |
| `object()` | Membuat objek kosong paling dasar. | `obj = object()` |
| `type(obj)` | Mengembalikan tipe dari sebuah objek. | `type(123)` → `<class 'int'>` |
| `vars(obj)` | Mengembalikan atribut `__dict__` suatu objek. | `vars(my_obj)` |

---

## 🛠️ 6. Manipulasi Atribut & Scope
Berinteraksi dengan variabel dan atribut secara dinamis.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `delattr(o, n)` | Menghapus atribut dari sebuah objek. | `delattr(p, 'name')` |
| `getattr(o, n)` | Mendapatkan nilai atribut secara dinamis. | `getattr(x, 'y')` |
| `globals()` | Mengembalikan dictionary variabel global saat ini. | `globals()` |
| `hash(obj)` | Mendapatkan nilai hash dari sebuah objek. | `hash("abc")` |
| `locals()` | Mengembalikan dictionary variabel lokal saat ini. | `locals()` |
| `setattr(o, n, v)`| Mengatur nilai atribut secara dinamis. | `setattr(x, 'y', 10)` |

---

## 🏗️ 7. Class & Method Decorators
Fungsi khusus untuk pengembangan berbasis objek (OOP).

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `classmethod(m)` | Mengubah metode menjadi class method. | `@classmethod` |
| `property(...)` | Membuat getter/setter/deleter untuk atribut. | `@property` |
| `staticmethod(m)`| Mengubah metode menjadi static method. | `@staticmethod` |
| `super()` | Mengakses metode dari parent class. | `super().__init__()` |

---

## ⚡ 8. Eksekusi Dinamis
**Gunakan dengan hati-hati!** Menjalankan kode dari string.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `compile(...)` | Mengompilasi source menjadi objek kode/AST. | `compile('a=5', '', 'exec')` |
| `eval(expr)` | Mengevaluasi ekspresi Python dari string. | `eval("1 + 2")` → `3` |
| `exec(object)` | Mengeksekusi kode Python secara dinamis. | `exec("print('Halo')")` |
| `__import__(n)` | Fungsi internal yang dipanggil oleh `import`. | `__import__('os')` |

---

## 🌐 9. I/O & Interaksi Sistem
Berkomunikasi dengan pengguna dan sistem file.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `breakpoint()` | Menjalankan debugger di titik tersebut. | `breakpoint()` |
| `help(obj)` | Menampilkan sistem bantuan interaktif. | `help(len)` |
| `input(p)` | Membaca input dari keyboard sebagai string. | `name = input("Nama: ")` |
| `open(f, m)` | Membuka file untuk dibaca/ditulis. | `open("test.txt", "r")` |
| `print(*obj)` | Mencetak objek ke output standar. | `print("Halo Dunia")` |

---

## ⏳ 10. Async & Miscellaneous
Fungsi untuk pemrograman asinkron dan lainnya.

| Fungsi | Deskripsi | Contoh |
| :--- | :--- | :--- |
| `aiter(async_it)`| Versi asinkron dari `iter()`. | `aiter(my_async_gen)` |
| `anext(async_it)`| Versi asinkron dari `next()`. | `await anext(it)` |
| `memoryview(obj)`| Mengakses memori objek tanpa menyalin data. | `memoryview(b'abc')` |

---
## Referensi
- [Official Python Documentation - Built-in Functions](https://docs.python.org/3/library/functions.html)
- Rishikant Sharma - "All 71 Python Built-in Functions Explained"
