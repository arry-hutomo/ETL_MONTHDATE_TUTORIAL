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

# 📚 Panduan Lengkap Setup Anaconda & UV Environment untuk Data Science/AI


Berikut adalah panduan lengkap untuk setup environment data science/AI menggunakan Anaconda dan UV Environment. Tutorial ini dibuat dengan penjelasan step-by-step yang mudah diikuti.

---

## Apa Itu Anaconda dan Conda?

**Anaconda** adalah distribusi open-source untuk bahasa pemrograman Python dan R, yang dirancang untuk komputasi ilmiah, analisis data, dan pembelajaran mesin. Anaconda menyederhanakan manajemen paket dan lingkungan, serta mendukung lebih dari 1.500 paket data science yang siap pakai.  

**Conda** adalah manajer paket dan lingkungan yang disertakan dalam Anaconda. Conda memungkinkan pengguna untuk mengelola paket dan lingkungan secara efisien, menghindari konflik dependensi, dan memastikan konsistensi proyek.

---

## ❓ Mengapa Kita Membutuhkan Virtual Environment?

Lingkungan virtual memungkinkan kita untuk:

- Mengisolasi proyek: Setiap proyek memiliki dependensi dan versi paket yang spesifik tanpa mempengaruhi proyek lain.
- Mencegah konflik versi: Menghindari masalah yang muncul ketika dua proyek memerlukan versi paket yang berbeda.
- Reproduksibilitas: Memastikan bahwa kode dapat dijalankan dengan dependensi yang konsisten di berbagai sistem.

---

## Apa Itu UV?

UV adalah alat manajemen lingkungan Python yang memungkinkan pembuatan, pengelolaan, dan penghapusan lingkungan virtual dengan mudah. Berbeda dengan pip dan virtualenv, UV mengintegrasikan pembuatan lingkungan dan instalasi paket dalam satu perintah, serta menyediakan pengelolaan versi Python secara otomatis.

---

## Mengapa Menggunakan UV?

- **Kecepatan**: Instalasi paket dan resolusi dependensi yang lebih cepat dibandingkan dengan pip dan poetry.
- **Kemudahan Penggunaan**: Perintah yang sederhana dan intuitif untuk pembuatan dan pengelolaan lingkungan.
- **Manajemen Versi Python**: Kemampuan untuk mengelola berbagai versi Python tanpa memerlukan alat tambahan.
- **Isolasi Proyek**: Setiap proyek dapat memiliki lingkungan dan dependensi yang terpisah, menghindari konflik antar proyek.

---

## 🐍 Bagian 1: Instalasi Anaconda

**1. Download Installer Anaconda**
   **Apa**
   File installer untuk memasang Anaconda ke komputer Anda.
   **Kenapa**
   Anaconda menyediakan Python dan paket data science siap pakai dalam satu instalasi.

   Langkah-langkah:
    - Buka https://www.anaconda.com/products/distribution
    - Pilih versi sesuai OS Anda (Windows/macOS/Linux)
    - Klik tombol Download

![image](https://github.com/user-attachments/assets/901655f0-1af9-4488-95aa-1ad47e7f3c1f)
   
   Do's:
	- Download dari situs resmi Anaconda
	- Simpan installer di folder yang mudah diakses
   Don'ts:
	- Jangan download dari sumber tidak resmi
	- Jangan simpan di folder system

**2. Jalankan Installer Anaconda**
   **Apa**
   Proses pemasangan Anaconda ke sistem Anda.
   **Kenapa**
   Untuk mendapatkan Python dan semua paket data science yang dibutuhkan.

   Langkah-langkah:
	- Buka file installer yang sudah didownload
	- Ikuti wizard instalasi
	- Pilih opsi "Add Anaconda to PATH" (opsional)

![image](https://github.com/user-attachments/assets/5f595980-7491-4c59-89c5-2f13c614ba8f)
 
   Do's:
	- Gunakan pengaturan default jika tidak yakin
	- Centang opsi PATH jika ingin bisa diakses dari terminal manapun
   Don'ts:
	- Jangan ubah direktori instalasi ke folder sistem
	- Jangan batalkan proses instalasi di tengah jalan

**3. Verifikasi Anaconda Terinstall dan Dapat Diakses**
    **Apa?**
    Verifikasi ini memastikan bahwa Anaconda sudah benar-benar terpasang dan bisa dipanggil dari terminal.
    **Kenapa?**
    Agar kita tidak menemui masalah di langkah selanjutnya saat menggunakan conda atau Python dari Anaconda.

    Langkah-langkah:
    1. Buka terminal atau command prompt.
    2. Ketik perintah:
       conda --version
    3. Jika muncul versi conda, instalasi sudah sukses.

![image](https://github.com/user-attachments/assets/e1a4a445-fc96-4e90-b66a-7975f39b1cdd)
    
    Do's:
    - Gunakan terminal baru setelah instalasi untuk memastikan variabel PATH terbaru terbaca   - Pastikan perintah dijalankan tanpa error.
    Don'ts:
    - Jangan abaikan error atau tidak muncul versi, cek pemasangan kembali.

**4. Konfigurasi Variabel Lingkungan PATH Conda dan Anaconda**
    **Apa?**
    Pengaturan variabel lingkungan PATH supaya perintah conda dan python dari Anaconda dapat diakses dari terminal manapun.
    **Kenapa?**
    Agar kita tidak harus selalu membuka Anaconda Navigator atau terminal khusus untuk menjalankan conda atau Python.

    Langkah-langkah:
    1. Pada Windows, tambahkan direktori Anaconda dan Scripts ke PATH Environment Variable.
    2. Pada macOS/Linux, biasanya otomatis terpasang. Jika tidak, edit .bashrc atau .zshrc untuk menambah PATH
    3. Tekan Windows + R, ketik sysdm.cpl, tekan Enter.
    4. Pergi ke tab "Advanced", klik "Environment Variables".
    5. Pilih "Path" di "System variables", klik "Edit".
    6. Tambahkan (ganti NAMA_ANDA):
    7. Klik Ok

![image](https://github.com/user-attachments/assets/f503738e-510e-419e-9a72-dce9d00fd668)

    Do's:
    - Pastikan sudah menutup dan membuka terminal baru setelah konfigurasi.
    - Restart komputer jika perlu.

    Don'ts:
    - Jangan menghapus PATH penting lainnya.
    - Hati-hati saat edit variabel lingkungan.
    
  
**5. Membuat Lingkungan Conda Baru**
    **Apa?**
    Membuat environment Conda baru adalah membuat ruang kerja terpisah untuk project yang berbeda.
    **Kenapa?**
    Untuk menghindari bentrok antar versi Python atau paket yang digunakan oleh berbagai proyek.

    Langkah-langkah:
    - Jalankan perintah berikut di terminal: conda create -n nama_env python=3.9
 
![image](https://github.com/user-attachments/assets/d70ace8b-3a0c-45b6-85a5-cf87a575e5da)

    Do's:
    - Gunakan nama environment yang deskriptif dan mudah diingat.
    - Jangan buat environment tanpa kebutuhan.

    Don'ts:
    - Jangan install semua paket di environment base.

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
**Apa:** Lingkungan Conda merupakan ruang kerja sendiri untuk suatu proyek

**Kenapa:** Lingkungan Conda perlu dibuat agar tidak bentrok dengan proyek lain (dependesi)
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
Install UV dengan mengetikan di command prompt: pip install uv

Jika berhasil versi UV akan tampil dan ada keterangan sukses

![instalasi_UV](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Install%20UV%20berhasil.png)

#### B. Menginisialisasi Proyek dalam UV
Tentukan direktori proyek yang akan digunakan, buat di command prompt dengan mengetikan init nama_direk

![aktivasi uv](https://github.com/Agus-Iskandar-D/ETL_MONTHDATE_TUTORIAL/blob/Tugas-Agus/Inisialisasi%20UV%20(1).png)

Buat lingkungan UV, ketik di command prompt: uv venv

Aktifkan dengan mengetikan: .venv\Scripts\activate

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
---