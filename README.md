# Sistem Pengelolaan Nilai Mahasiswa Menggunakan Array
## Deskripsi Project

Project ini merupakan implementasi sederhana dari konsep struktur data array menggunakan bahasa pemrograman Python. Program dibuat untuk mengelola nilai mahasiswa dengan beberapa fitur analisis data dan visualisasi grafik.

- Program ini memiliki fitur utama:
- Input 10 nilai mahasiswa
- Menampilkan daftar nilai
- Menampilkan nilai tertinggi
- Menampilkan nilai terendah
- Menghitung rata-rata nilai
- Menghitung jumlah mahasiswa lulus (nilai ≥ 60)
- Menampilkan grafik perbandingan nilai tertinggi dan terendah
- Menampilkan grafik persentase kelulusan mahasiswa

Program dijalankan menggunakan Python di Google Colab dan hasil visualisasi dibuat menggunakan library Matplotlib.

# 1. Penjelasan Konsep Array

Array adalah struktur data yang digunakan untuk menyimpan sekumpulan data dalam satu variabel dengan tipe yang sama. Dalam Python, array biasanya diimplementasikan menggunakan list.

Contoh sederhana array pada Python:

`nilai = [96, 91, 86, 81, 76]`

Pada program ini, array digunakan untuk menyimpan nilai mahasiswa yang dimasukkan oleh pengguna.

Contoh implementasi pada program:
```
nilai = []

for i in range(10):
    n = int(input(f"Masukkan nilai ke-{i+1}: "))
    nilai.append(n)
```
Penjelasan:

- `nilai = []` membuat array kosong
- `for i in range(10)` melakukan perulangan sebanyak 10 kali
- `append()` digunakan untuk menambahkan nilai ke dalam array

Setelah semua nilai dimasukkan, array tersebut digunakan untuk melakukan beberapa proses analisis seperti:

- mencari nilai tertinggi
- mencari nilai terendah
- menghitung rata-rata
- menghitung jumlah mahasiswa yang lulus

Dengan menggunakan array, pengolahan data menjadi lebih mudah karena semua nilai tersimpan dalam satu struktur data.
