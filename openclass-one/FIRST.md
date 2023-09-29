# Open Class: Learn the Essential Foundations

**LEARNING OUTLINE**
* Computational Thinking
* Programming Basic
* Git & Github
---
### APA ITU COMPUTATIONAL THINKING?
> Sederhananya, **Computational Thinking** adalah kemampuan untuk memecahkan masalah kompleks dengan menggunakan prinsip-prinsip pemrograman dan logika komputasi.

**Terdapat 4 landasan utama pada konsep Computational Thinking**
1. Decomposition (Dekomposisi)
2. Pattern recognition (Pengenalan Pola)
3. Abstraction (Abstraksi)
4. Algorithms (Algoritma)

### A. Decomposition (Dekomposisi)
> Proses mengurai masalah yang kompleks menjadi bagian-bagian kecil sehingga lebih mudah untuk ditangani.

![Dekomposisi](../img/dekomposisi.png)

**Analogi Dekomposisi Ketika Menyeduh Kopi**
* **Mempersiapkan Air Panas:** Memanaskan air dengan suhu yang tepat
* Membuka kemasan kopi
* Menempatkan kopi sachet dalam cangkir
* **Menuangkan Air Panas:** Menuangkan air panas ke dalam cangkir berisi kopi sachet
* **Mengaduk Kopi (Opsional):** Aduk kopi agar merata
* Hidangkan kopi

**Contoh Dekomposisi Dalam Pemrograman Python:**
```python
# Langkah 1: Mempersiapkan Air Panas
def mempersiapkan_air():
    print("Panaskan air hingga mendidih.")

# Langkah 2: Memilih Kopi Sachet
def memilih_kopi():
    print("Pilih sachet kopi favorit Anda.")

# Langkah 3: Membuka Sachet
def membuka_sachet():
    print("Buka kemasan sachet kopi dengan hati-hati.")

# Langkah 4: Menyeduh Kopi
def menyeduh_kopi():
    print("Masukkan sachet kopi ke dalam cangkir.")
    print("Tuangkan air panas ke dalam cangkir dengan sachet kopi.")
    print("Aduk perlahan untuk memastikan kopi tercampur dengan baik.")

# Langkah 5: Menikmati Kopi
def menikmati_kopi():
    print("Angkat sachet kopi dan nikmati secangkir kopi yang nikmat.")

# Implementasi Seluruh Proses
def menyeduh_kopi_sachet():
    mempersiapkan_air()
    memilih_kopi()
    membuka_sachet()
    menyeduh_kopi()
    menikmati_kopi()

# Panggil Fungsi Utama
menyeduh_kopi_sachet()
```
> Pada contoh program di atas, setiap langkah dipecah ke dalam beberapa prosedur sehingga lebih memudahkan untuk diolah, diproses, dan dipahami. Coba bayangkan kalau kamu menyatukan seluruh proses di atas tanpa memecah setiap bagiannya, maka tentu saja program akan terlihat terlalu kompleks dan sulit untuk dipahami.

---

### B. Pattern recognition (Pengenalan Pola)
> Mencari dan menganalisa persamaan atau pola yang terdapat di dalam suatu permasalahan.

**Perhatikan Gambar Berikut!**
![Dekomposisi](../img/pattern.png)
>Apa yang berhasil kamu tangkap dari gambar tersebut?

**Analogi: Pola pada Deret Angka**

Bayangkan kamu memiliki deret angka berikut: `2, 4, 6, 8, 10.`

Dalam deret ini, kita bisa mengenali bahwa setiap angka berikutnya merupakan angka genap dan hasil penambahan 2 dari angka sebelumnya (kelipatan 2).
Misal, `2 + 2 = 4`, `4 + 2 = 6`, `6 + 2 = 8` dan seterusnya.

> Dengan penerapan **pattern recognition**, kita bisa dengan cepat mengidentifikasi hubungan atau aturan tertentu di antara elemen-elemen suatu set atau deret data (berlaku juga untuk permasalahan lain secara luas). Dengan begitu, kita bisa dengan lebih mudah untuk memahami dan memprediksi apa yang akan terjadi selanjutnya.

**Contoh Pattern Recognition Dalam Pemrograman Python**
```python
# Fungsi untuk Mengenali Pola pada Deret Angka
def mengenali_pola(deret):
    pola = deret[1] - deret[0]  # Menghitung pola dari selisih elemen pertama dan kedua
    for i in range(1, len(deret)-1):
        if deret[i+1] - deret[i] != pola:
            return None  # Jika selisih antar elemen tidak sama, maka tidak ada pola
    return pola

# Deret Angka
deret_angka = [2, 4, 6, 8, 10]

# Mengenali Pola pada Deret Angka
hasil_pola = mengenali_pola(deret_angka)

# Menampilkan Hasil
if hasil_pola is not None:
    print(f"Pola deret angka adalah penambahan {hasil_pola}")
else:
    print("Tidak ada pola yang teridentifikasi dalam deret angka.")
```
**Bedah Program:**
1. Fungsi `mengenali_pola` akan menerima sebuah deret angka dan mencoba mengenali pola di antara elemen-elemennya.
2. Program akan memeriksa apakah selisih antar elemen berurutan adalah konstan. Jika iya, maka program akan mengembalikan pola penambahan tersebut.
3. Dalam contoh deret angka `[2, 4, 6, 8, 10]`, program akan mengenali pola sebagai penambahan 2.
4. Hasil dari pengenalan pola akan ditampilkan.
   
> Jika kamu ingin mencoba dengan deret angka lain, cukup ubah nilai pada variabel `deret_angka` sesuai keinginanmu. Misalnya, deret_angka = `[3, 6, 9, 12, 15]` akan menghasilkan pola penambahan 3.

---

### C. Abstraction (Abstraksi)
> Fokus pada informasi yang penting saja dan mengabaikan informasi lain yang tidak relevan

### D. Algorithms (Algoritma)
> Urutan langkah-langkah sistematis, logis dan efektif untuk menyelesaikan suatu permasalahan.
