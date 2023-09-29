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
```
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

### B. Pattern recognition (Pengenalan Pola)
> Mencari dan menganalisa persamaan atau pola yang terdapat di dalam suatu permasalahan.

### C. Abstraction (Abstraksi)
> Fokus pada informasi yang penting saja dan mengabaikan informasi lain yang tidak relevan

### D. Algorithms (Algoritma)
> Urutan langkah-langkah sistematis, logis dan efektif untuk menyelesaikan suatu permasalahan.
