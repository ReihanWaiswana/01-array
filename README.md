# 📝 Sistem Pengelolaan Nilai Mahasiswa Menggunakan Array
## 💡 Deskripsi Project

Project ini merupakan implementasi sederhana dari konsep struktur data array menggunakan bahasa pemrograman Python. Program dibuat untuk mengelola nilai mahasiswa dengan beberapa fitur analisis data dan visualisasi grafik.

### Program ini memiliki fitur utama:
- Input 10 nilai mahasiswa
- Menampilkan daftar nilai
- Menampilkan nilai tertinggi
- Menampilkan nilai terendah
- Menghitung rata-rata nilai
- Menghitung jumlah mahasiswa lulus (nilai ≥ 60)
- Menampilkan grafik perbandingan nilai tertinggi dan terendah
- Menampilkan grafik persentase kelulusan mahasiswa

Program dijalankan menggunakan Python di Google Colab dan hasil visualisasi dibuat menggunakan library Matplotlib.

# 1. Penjelasan Konsep Array 📄

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

# 2. Screenshot Hasil Eksekusi Program 📷

## Soal_01

Berikut adalah hasil eksekusi program pada Google Colab.

### - Input Nilai Mahasiswa 

Program meminta pengguna untuk memasukkan 10 nilai mahasiswa.

Contoh input pada program:

<img width="251" height="235" alt="image" src="https://github.com/user-attachments/assets/cdbb44cb-eea6-4b8c-bd4d-7ab6d05e0420" />

### - Output Program

Setelah data dimasukkan, program akan menampilkan hasil analisis:

<img width="667" height="165" alt="image" src="https://github.com/user-attachments/assets/c505f32d-784e-4af9-935e-e97acc0fae78" />

## Soal_02

### - Grafik Perbandingan Nilai Tertinggi & Terendah 

Program menampilkan grafik batang untuk memperlihatkan perbandingan antara nilai tertinggi dan nilai terendah mahasiswa.

<img width="571" height="435" alt="image" src="https://github.com/user-attachments/assets/ffbdf00e-48c2-43ec-b522-519acb651fe8" />

Grafik ini membantu memvisualisasikan perbedaan nilai secara lebih jelas.

### - Grafik Persentase Kelulusan

Program juga menampilkan grafik pie yang menunjukkan persentase mahasiswa yang lulus dan tidak lulus.

Pada contoh data:
- 7 mahasiswa lulus
- 3 mahasiswa tidak lulus

Sehingga persentase kelulusan adalah:

<img width="515" height="411" alt="image" src="https://github.com/user-attachments/assets/3ef0ba23-c701-4bd4-8860-022032ed29f7" />

- Lulus : 70%
- Tidak Lulus : 30%

# 3. Analisis Kompleksitas Algoritma 🔎

Analisis kompleksitas digunakan untuk mengetahui efisiensi suatu algoritma berdasarkan jumlah data yang diproses.

Dalam analisis ini digunakan notasi **Big O Notation**.

## Soal_01

### - Input Nilai Mahasiswa

    for i in range(10):

**Kompleksitas waktu:**

`O(n)`

Karena program melakukan proses input sebanyak jumlah data yang dimasukkan.

### - Menampilkan Nilai Tertinggi

    max(nilai)

**Kompleksitas waktu:**

`O(n)`

Karena fungsi `max()` harus memeriksa seluruh elemen dalam array untuk menentukan nilai terbesar.

### - Menampilkan Nilai Terendah

    min(nilai)

**Kompleksitas waktu:**

`O(n)`

Karena fungsi `min()` harus memeriksa semua elemen dalam array untuk menentukan nilai terkecil.

### - Menghitung Rata-Rata
    
    sum(nilai)/len(nilai)

**Kompleksitas waktu:**

`O(n)`

Karena fungsi `sum()` menjumlahkan seluruh elemen dalam array.

### - Menghitung Jumlah Mahasiswa Lulus
    for n in nilai:
        if n >= 60:
            lulus += 1

**Kompleksitas waktu:**

`O(n)`

Karena program harus memeriksa setiap nilai mahasiswa satu per satu.

## Soal_02

### - Inisialisasi Array

    nilai = np.array([90, 78, 98, 56, 67, 54, 70, 60, 49, 95])

**Kompleksitas waktu:**

`O(1)`

Karena array dibuat langsung dengan nilai yang sudah ditentukan sebelumnya. Karena jumlah elemen bersifat tetap (10 nilai), maka proses ini memiliki kompleksitas konstan dan tidak bergantung pada ukuran input.

### - Print array

    print("Daftar Nilai :", nilai)

**Kompleksitas waktu:**

`O(1)`

Karena hanya menampilkan data.

### - Menghitung jumlah mahasiswa tidak lulus

    tidakLulus = len(nilai) - lulus

**Kompleksitas waktu:**

`O(1)`

Karena operasi ini hanya melakukan pengurangan antara jumlah total mahasiswa dengan jumlah mahasiswa yang lulus. Fungsi `len()` pada Python memiliki kompleksitas `O(1)` karena panjang array sudah tersimpan dalam struktur data.

### - Pembuatan Grafik

Pembuatan grafik menggunakan library Matplotlib memiliki kompleksitas yang relatif kecil terhadap jumlah data sehingga dapat dianggap:

`O(1)`

Pembuatan grafik menggunakan Matplotlib memiliki kompleksitas `O(1)` karena jumlah data yang divisualisasikan tetap (nilai tertinggi, nilai terendah, jumlah lulus, dan tidak lulus). Jumlah elemen pada grafik tidak bertambah meskipun jumlah data mahasiswa meningkat.

# 4. Refleksi Pembelajaran 📘

Saya mempelajari beberapa konsep penting tentang struktur data dan pemrograman selama tugas ini.

Pertama, saya belajar bagaimana list, atau array, mempermudah proses pengolahan data dengan menyimpan banyak data dalam satu variabel.

Saya juga belajar cara membaca data pengguna dan melakukan proses analisis dengan menggunakan loop.

Selain itu, saya mempelajari bagaimana menghitung nilai statistik sederhana seperti:

- Nilai tertinggi
- Nilai terendah
- Rata-rata
- Jumlah mahasiswa yang lulus

Menurut saya tugas ini sangat menarik karena penggunaan grafik untuk menunjukkan data sehingga hasil analisis lebih mudah dipahami.

Salah satu praktik penting dalam pengembangan perangkat lunak adalah penggunaan **GitHub** untuk menyimpan project dan melakukan commit secara bertahap, hal tersebut juga saya pelajari dalam pembelajaran ini.

Melalui tugas ini, saya meningkatkan pemahaman saya tentang bagaimana konsep struktur data dapat digunakan untuk menyelesaikan masalah pengolahan data yang lebih sederhana.
