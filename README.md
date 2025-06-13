# Setup Anaconda, Conda, dan UV
----
## 🚀 Intro 

**Anaconda** merupakan platform distribusi project data science, machine leaning, dan AI dalam bahasa pemrograman pyhton dan R. Sedangkan, **Conda** manajer paket dan lingkungan open-source yang merupakan bagian inti dari Anaconda. Meskipun sering dikaitkan dengan Anaconda, Conda juga bisa digunakan secara mandiri (misalnya melalui Miniconda, versi minimal Anaconda). Sementara itu, **UV** merupakan manajer paket Python modern yang relatif baru, dibangun dengan bahasa Rust. Berikut perbedaan ketiganya:

![perbandingan](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/perbedaan%20anaconda%2C%20conda%2C%20UV.png)

## 🌱 Kenapa Harus Ketiganya? 
1. Ketiganya open-source.
2. Anaconda menjadi pilihan karena ia menyediakan fondasi yang kokoh dan komprehensif library esensial yang lengkap.
3. Conda mampu mengelola semua dependensi ini secara terpadu. 
4. UV mampu mempercepat instalasi paket Python di dalam lingkungan Conda.
## Ketiganya memberikan kemudahan setup, fleksibilitas manajemen lingkungan, dan kecepatan eksekusi.

----

## ⚙️ Langkah-langkah Setup 

### Setup Anaconda
---
Kamu bisa mengunduh instaler anaconda di web anaconda
![web_anaconda](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/web%20anaconda.png)

1. Unduh installer Anaconda3-2024.10-1-Windows-x86_64.exe.

![installer](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/instalaser%20anaconda.png)

2. Install dengan cara double klik
3. Klik "Next" pada layar sambutan.
4. Setujui syarat lisensi.

![lisensi](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Centang%20Agreement.png)

5. Pilih "Just Me (recommended)".
6. Gunakan lokasi default (C:\Users\NAMA_ANDA\anaconda3).

![lokasi](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Lokasi.png)

7. Centang Anaconda3 ke PATH.

![centang](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Centang%20path.png)

8. Klik "Install" dan tunggu selesai.
![proses_intalasi](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/berhasil%20install%202.png)

**DOs**: Centang PATH pada proses Instalasi, lakukan setup PATH secara manual

**Don'ts**: Jangan lakukan double instalasi

---

### Verifikasi Anaconda
----
1. Buka command prompt
2. Ketik Conda --version
3. Output seperti conda 24.1.0 menunjukkan keberhasilan.

![berhasil](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/verifikasi%20anaconda.png)

----

### Setup (Aktivasi) Conda
----
#### A. Membuat lingkungan baru Conda
Apa: Lingkungan Conda merupakan ruang kerja sendiri untuk suatu proyek
Kenapa: Lingkungan Conda perlu dibuat agar tidak bentrok dengan proyek lain (dependesi)
1. Pada command prompt ketik conda create -n name_env python=9.12 (pada contoh: test_4)
2. pilih y

#### B. Mengaktifkan Lingkungan Conda
Aktifkan lingkungan conda dengan mengetik pada command prompt conda activate name_env

![aktivasi_conda](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Aktivasi%20conda%20(2).png)

#### C. Menginstall Paket
Install paket library sesuai kebutuhan, pada command prompt ketik pip install pandas (contoh: pandas)

![install_paket](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/install%20paket%20conda.png)

#### D. Menonaktifkan Lingkungan Conda
Nonaktifkan lingkungan conda dengan mengetik pada command prompt conda deactivate

![nonaktif_conda](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/deaktivasi%20conda.png)

**Do:** Berikan nama lingkungan yang relevan
**Dont:** Jangan intall semua paket, tapi install sesuai kebutuhan

-----

### Setup (Aktivasi) UV
-----
#### A. Install UV
install UV dengan mengetikan di command prompt pip install uv
Jika berhasil versi UV akan tampil dan ada keterangan sukses

![instalasi_UV](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Install%20UV%20berhasil.png)

#### B. Menginisialisasi Proyek dalam UV
Tentukan direktori proyek yang akan digunakan, buat di command prompt dengan mengetikan init nama_direk

![aktivasi uv](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Inisialisasi%20UV%20(1).png)

Buat lingkungan UV, ketik di command prompt: uv venv
aktifkan dengan mengetikan: .venv\Scripts\activate

#### C. Menginstall Paket Librari
Ketikan uv add nama paket (contoh: uv add pandas)

#### D. Menonaktifkan Lingkungan UV
ketikan .venv\Scripts\deactivate

![aktivasi_dan_install](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Aktivasi%20dan%20install%20paket.png)

**Dos:** Pastikan direktorinya jelas dan UV aktif saat install librari
**Donts:** Jangan install paket librari yang tidak dibutuhkan

-----

## Kesimpulan

![anaconda,uv](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/anaconda%2C%20conda%2C%20UV.png)

Jika dianalogikan, **Anaconda** adalah Kota lengkap tempat para ilmuwan dan engineer data bekerja, sedangkan **Conda** adalah Manajer apartemen dan gudang di kota itu, yang mengatur lingkungan proyek agar tidak saling mengganggu dan memastikan semua alat bekerja sama. Semantara itu, **UV** adalah Kurir super cepat yang mengantar paket-paket Python dengan efisiensi dan kecepatan luar biasa.

### Dengan menggunakan ketiganya kita akan:
1. Menghindari konflik versi antar paket. ✅
2. Memastikan konsistensi dan reproduktibilitas hasil. 🔄
3. Mengelola dependensi secara efisien, terutama pada proyek kompleks. ⚙️
