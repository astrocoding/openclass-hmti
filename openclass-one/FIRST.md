# Open Class: Learn the Essential Foundations

**LEARNING OUTLINE**
* Computational Thinking
* Programming Basic
* Git & Github
---
### APA ITU COMPUTATIONAL THINKING?
> Sederhananya, **Computational Thinking** adalah kemampuan untuk memecahkan masalah kompleks dengan menggunakan prinsip-prinsip pemrograman dan logika komputasi.

![Computational Thinking](../img/computational_thinking.jpg)

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
![Pattern Recognition](../img/pattern.png)
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

![Abstraction](../img/abstraction.webp)

**Analogi: Pemilihan Playlist Musik**

Bayangkan kamu sedang menggunakan aplikasi musik seperti Spotify dan ingin memilih playlist untuk suasana hati tertentu, misalnya "Santai". Ketika kamu memilih playlist "Santai", kamu sebenarnya tidak perlu tahu setiap lagu yang ada di dalamnya atau bagaimana dibuatnya. Kamu hanya perlu tahu bahwa playlist ini cocok untuk suasana hati santai.

Nah, dalam kasus ini kamu telah melakukan abstraksi terhadap kumpulan lagu dalam playlist. Kamu tidak perlu sampai memikirkan detail dari setiap lagu, tetapi cukup menggunakan abstraksi "Playlist Santai" untuk mencapai tujuanmu **(Mendengarkan musik santai)**.

> Dalam Computational Thinking, **abstraction** memungkinkan kita untuk fokus pada informasi yang penting saja dan mengabaikan detail yang tidak relevan. Seperti dalam contoh ini, kamu fokus pada tujuan akhir (mendengarkan musik santai) tanpa harus tahu semua lagu di dalam playlist tersebut.

**Contoh Abstraction Dalam Pemrograman Python:**
```python
# Daftar Playlist Musik
playlist_santai = ["Lagu Santai 1", "Lagu Santai 2", "Lagu Santai 3", "Lagu Santai 4"]
playlist_energik = ["Lagu Energi 1", "Lagu Energi 2", "Lagu Energi 3", "Lagu Energi 4"]

# Fungsi untuk Memilih Playlist
def pilih_playlist(suasana_hati):
    if suasana_hati == "santai":
        return playlist_santai
    elif suasana_hati == "energik":
        return playlist_energik
    else:
        return []

# Meminta Input Suasana Hati dari Pengguna
suasana_hati = input("Masukkan suasana hati Anda (santai / energik): ")

# Memilih Playlist Sesuai Suasana Hati
playlist_terpilih = pilih_playlist(suasana_hati)

# Menampilkan Playlist Terpilih
if playlist_terpilih:
    print(f"Playlist {suasana_hati}:")
    for lagu in playlist_terpilih:
        print(f"- {lagu}")
else:
    print("Playlist tidak ditemukan.")
```
**Bedah Program:**
1. Program memiliki dua daftar playlist: `playlist_santai` dan `playlist_energik`.
2. Fungsi `pilih_playlist` menerima input `suasana_hati` dan mengembalikan playlist sesuai dengan suasana hati yang diminta.
3. Pengguna diminta untuk memasukkan suasana hati mereka (santai atau energik).
4. Program memilih playlist berdasarkan input pengguna dan menampilkannya.
5. Misalnya, jika pengguna memasukkan "santai", program akan menampilkan playlist santai. Jika pengguna memasukkan sesuatu selain "santai" atau "energik", program akan memberikan pesan bahwa playlist tidak ditemukan.

---

### D. Algorithms (Algoritma)
> Urutan langkah-langkah sistematis, logis dan efektif untuk menyelesaikan suatu permasalahan.

![Algorithms](../img/algoritma.jpg)

**Algoritma: Membuat Roti Panggang**
1. Siapkan roti tawar.
2. Panggang roti hingga kecoklatan di oven atau pemanggang roti.
3. Setelah roti matang, angkat dari oven atau pemanggang.
4. Olesi permukaan roti dengan mentega.
5. Olesi permukaan roti dengan selai strawberry.
6. Letakkan roti di atas piring.
7. Sajikan roti panggang.

**Contoh Algoritma Sederhana Dalam Python:**
```python
# Fungsi untuk Membuat Roti Panggang
def buat_roti_panggang():
    print("1. Siapkan roti tawar.")
    print("2. Panggang roti hingga kecoklatan di oven atau pemanggang roti.")
    print("3. Setelah roti matang, angkat dari oven atau pemanggang.")
    print("4. Olesi permukaan roti dengan mentega.")
    print("5. Olesi permukaan roti dengan selai strawberry.")
    print("6. Letakkan roti di atas piring.")
    print("7. Sajikan roti panggang.")

# Memanggil Fungsi untuk Membuat Roti Panggang
buat_roti_panggang()
```
---
### PEMROGRAMAN DASAR DENGAN PYTHON
> Pemrograman adalah proses membuat rangkaian instruksi atau algoritma yang ditulis dalam bahasa yang dapat dimengerti oleh komputer.

**COMPILER DAN INTERPRETER**
> **Compiler** adalah program komputer yang menerjemahkan kode sumber keseluruhan ke dalam bahasa mesin atau kode biner. Proses ini menghasilkan file yang dapat dieksekusi secara independen tanpa memerlukan compiler lagi setiap kali program dijalankan.

Sedangkan

> **Interpreter** adalah program komputer yang mengeksekusi kode sumber secara baris per baris tanpa menghasilkan file terpisah. Setiap baris dieksekusi secara langsung saat program berjalan.

**KONSEP DALAM PEMROGRAMAN DASAR**
1. **Variable dan Konstanta**
   > **Variable** Wadah/tempat untuk menyimpan data yang dapat berubah selama eksekusi program.
   > **Konstanta** Nilai yang tetap dan tidak dapat diubah selama eksekusi program.
    **Contoh Program:**
   ```python
   # Variable
   umur = 20
   nama = "Zaenal Alfian"
   # Konstanta
   PI = 3.14
   ```
2. **Tipe Data**
   > Jenis nilai yang dapat disimpan dalam sebuah variable atau konstanta. Contoh: `integer, float, string, boolean.`
   **Contoh Program:**
   ```python
   # Tipe Data Integer
   umur = 20
   # Tipe Data Float
   tinggi = 180.3
   # Tipe Data String
   nama = "Zaenal Alfian"
   # Tipe Data Boolean
   sudah_menikah = False
   ```
4. **Operator**
   > Simbol atau kata kunci yang digunakan untuk melakukan operasi pada data. Contoh: `+ (penjumlahan)`, `== (sama dengan)`, and `(logika AND)`.
   
   **Operator Aritmetika:**
   ```python
   # Operator Aritmetika
   a = 10
   b = 5

   penjumlahan = a + b
   pengurangan = a - b
   perkalian = a * b
   pembagian = a / b
   modulo = a % b
   pangkat = a ** b

   print(penjumlahan, pengurangan, perkalian, pembagian, modulo, pangkat)
   ```
   **Operator Perbandingan:**
   ```python
   # Operator Perbandingan
   x = 10
   y = 20

   lebih_besar = x > y
   kurang_dari = x < y
   sama_dengan = x == y
   tidak_sama_dengan = x != y
   lebih_besar_sama_dengan = x >= y
   kurang_dari_sama_dengan = x <= y

   print(lebih_besar, kurang_dari, sama_dengan, tidak_sama_dengan, lebih_besar_sama_dengan, kurang_dari_sama_dengan)
   ```
   **Operator Logika**
   ```python
   # Operator Logika
   p = True
   q = False

   and_operator = p and q
   or_operator = p or q
   not_operator_p = not p
   not_operator_q = not q

   print(and_operator, or_operator, not_operator_p, not_operator_q)
   ```
6. **Logika Perbandingan**
   > Membandingkan nilai atau ekspresi untuk menentukan kebenaran suatu pernyataan. Contoh: `> (lebih besar dari)`, `== (sama dengan)`, `!= (tidak sama dengan)`. Nilai yang dikembalikan adalah tipe data `boolean`
   **Contoh Program:**
   ```python
   umur = 18
   if umur < 18:
       print("Anda masih di bawah umur")
   elif umur == 18:
       print("Anda baru saja berusia 18 tahun")
   else:
       print("Anda sudah dewasa")
   ```
8. **Logika Perulangan**
   > Mengulang serangkaian instruksi sampai kondisi tertentu terpenuhi. Contoh: for loop, while loop, do while loop.
   **Contoh Program:**
   ```python
   # For Loop
   for i in range(5):
       print(i)
   
   # While Loop
   angka = 1
   while angka <= 5:
       print(angka)
       angka += 1
   ```
10. **Fungsi**
    > Blok kode yang dapat digunakan kembali untuk melakukan tugas tertentu. Didefinisikan dengan nama dan dapat menerima argumen/parameter
    **Contoh Program:**
    ```python
    def luas_persegi(sisi):
        return sisi * sisi

    luas = luas_persegi(4)
    print(f"luas persegi = {luas}")
    ```
12. **Struktur Data**
    > Cara untuk mengorganisasi dan menyimpan data agar dapat diakses dan dikelola dengan efisien. Contoh: `array`, `list`, `tuple`, `dictionary`.
    **Contoh Program:**
    ```python
    # List (Daftar)
    buah = ["apel", "jeruk", "mangga", "pisang"]

    # Tuple
    koordinat = (10, 20)

    # Dictionary
    mahasiswa = {"nama": "Zaenal Alfian", "umur": 20, "prodi": "Teknik Informatika"}
    ```
---
Credits: [Zaenal Alfian](https://github.com/astrocoding)
Last Edited on: 30/09/2023
