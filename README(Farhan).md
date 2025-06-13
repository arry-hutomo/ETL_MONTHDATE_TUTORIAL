
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


---

## 🧪 Bagian 2: Membuat UV Environment

**1. Buat Environment Baru**

    **Apa**
    Membuat environment terisolasi untuk proyek UV.
    
    **Kenapa**
    Agar dependensi proyek tidak bentrok dengan proyek lain.

    Langkah-langkah:
    1.	Pastikan lingkungan Conda tidak aktif (jalankan conda deactivate jika perlu).
    2.	Ketik: pip install uv
    3.	Output seperti Successfully installed uv-0.7.12 menunjukkan keberhasilan.
    4.	Catatan tentang folder ghost_intellixuv: Folder ghost_intellixuv akan dibuat di langkah berikutnya  menggunakan uv init. Perintah ini otomatis membuat folder jika belum ada, karena UV dirancang untuk menginisialisasi direktori proyek baru secara langsung. Anda tidak perlu membuat folder ini secara manual sebelum menjalankan uv init. Untuk memverifikasi folder setelah inisialisasi, ketik dir di CMD untuk melihat daftar direktori.

![image](https://github.com/user-attachments/assets/a5a483b1-87a4-4c7e-90ce-dcf3ee9943a7)

    Do's:
    - Beri nama environment yang deskriptif
    - Gunakan versi Python yang kompatibel
    Don'ts:
    - Jangan gunakan environment base untuk proyek
    - Jangan membuat terlalu banyak environment yang tidak perlu

**2. Menginisialisasi Proyek UV**

    **Apa?**
    Menginisialisasi Proyek UV adalah proses mempersiapkan struktur direktori dan file konfigurasi dasar untuk proyek yang akan menggunakan UV environment. Ini termasuk membuat file requirements, struktur folder, dan konfigurasi dasar proyek.
    
    **Kenapa?**
    Inisialisasi proyek yang benar membantu menjaga konsistensi struktur proyek, memudahkan kolaborasi tim, dan memastikan semua dependensi terkelola dengan baik. Ini juga mempermudah deployment dan reproduksi environment di mesin lain.
   
    Langkah-langkah:
    1. Pastikan environment UV sudah aktif
    2. Ketik: uv init ghost_intellixuv
               Cd ghost intellixuv
    3. Output menunjukkan proyek diinisialisasi di C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv.

![image](https://github.com/user-attachments/assets/17276dad-204c-4b2c-a3ef-e68214691642)
 
    Do's:
    - Gunakan struktur folder yang konsisten
    - Dokumentasikan semua dependensi di requirements.txt
    - Buat README.md yang jelas
    - Gunakan virtual environment untuk setiap proyek	

    Don'ts:
    - Jangan mencampur file proyek dengan file personal
    - Jangan lupa menambahkan environment ke .gitignore
    - Jangan menyimpan data sensitif di direktori proyek
    - Jangan mengubah struktur folder setelah proyek berjalan

**4. Install Paket yang Dibutuhkan**

    **Apa?**
    Memasang library yang diperlukan untuk proyek UV.
    
    **Kenapa?** 
    Untuk mendapatkan fungsi-fungsi yang dibutuhkan dalam pengembangan.
    
    Langkah-langkah:
    1.	Ketik: uv add pandas

![image](https://github.com/user-attachments/assets/61291641-7c48-4db3-b2b4-21958b056d76)

    Do's:
    - Install hanya paket yang diperlukan
    - Periksa versi paket yang kompatibel
    Don'ts:
    - Jangan install paket di environment base
    - Jangan install paket tanpa memeriksa dependensinya
    - Jangan campur UV dan pip.

 
**5. Menonaktifkan Lingkungan UV**
 
    **Apa?**
    Nonaktifkan environment uv_env apabila sudah selesai menggunakan.
    
    **Kenapa?**
    Agar shell kembali ke environment base atau default.

    Langkah-langkah:
    1.	Ketik: .venv\Scripts\deactivate
    2.	Prompt kembali ke C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>.

![image](https://github.com/user-attachments/assets/6017c6a5-06bb-4376-8248-d46fae0aece4)

    Do's:
    - Selalu deactivate ketika berpindah konteks.

    Don'ts:
    - Jangan tinggal aktif tanpa alasan.
    
  
**6. Perbandingan Conda vs UV**	

    **Apa?**
    Membandingkan manajemen environment Conda dengan framework UV (asumsi UV adalah sistem manajemen environment atau framework spesifik).
    
    **Kenapa?**
    Agar memudahkan pemilihan tools sesuai kebutuhan.
    
    Detail:
    - Conda: manajemen environment dan paket secara umum, lintas proyek.
    - UV: environment/framework yang lebih spesifik untuk proyek tertentu, mungkin terkait AI.

![image](https://github.com/user-attachments/assets/d4e68cf5-e066-44b5-bfb6-f070e9b755f1)

    Do's:
    - Gunakan Conda untuk manajemen environment yang luas.
    - Gunakan UV jika spesifik proyek atau framework tersebut.

    Don'ts:
    - Jangan mencampur konfigurasi environment yang berbeda tanpa sinkronisasi.
    
  
**7. Daftar Paket yang Direkomendasikan untuk UV Environment**
	
     Berikut daftar paket yang umum dan direkomendasikan dalam environment UV untuk data science dan machine learning:
    - numpy
    - pandas
    - matplotlib
    - scikit-learn
    - jupyter
    - seaborn
    - tensorflow atau pytorch (sesuai kebutuhan)

![image](https://github.com/user-attachments/assets/5020c54f-75e8-4036-b76f-d8882d712733)

    Do's:
    - Instal paket sesuai kebutuhan proyek.
    - Update paket secara berkala.

    Don'ts:
    - Jangan instal paket yang tidak dikenal tanpa keperluan.

  

**8. Panduan Pemecahan Masalah pada Conda dan UV**

    Masalah umum dan solusinya:
    Masalah 1: Perintah Conda Tidak Dikenali
    Gejala: 'conda' is not recognized
    Solusi:
   	- Verifikasi instalasi Anaconda.
   	- Periksa PATH.
   	- Jalankan conda init cmd.exe, mulai ulang terminal.

    Masalah 2: Aktivasi Lingkungan Gagal
    Gejala: Script execution is disabled
    Solusi:
   	- Jalankan PowerShell sebagai Administrator.
   	- Ketik Set-ExecutionPolicy RemoteSigned.
   	- Pilih "Y".

    Masalah 3: Kesalahan Instalasi Paket
    Gejala: Could not find a version
    Solusi:
   	- Perbarui pip: python -m pip install --upgrade pip.
   	- Periksa kompatibilitas Python.
   	- Coba versi paket lain.

    Do's:
    - Selalu baca dokumentasi dan pesan error.
    - Gunakan forum komunitas dan stackoverflow.

    Don'ts:
    - Jangan mengabaikan pesan error.
    - Jangan memaksa instalasi tanpa verifikasi.


---

## 🔄 Bagian 3: Manajemen Environment

Perintah-perintah Penting
Berikut beberapa perintah penting untuk mengelola environment:

![image](https://github.com/user-attachments/assets/5eec8061-abef-4564-b5eb-31bb6c6bcad6)

---

## 🎯 Kesimpulan

Anaconda ibarat kota besar yang terbagi menjadi gedung-gedung (environment) berbeda, masing-masing punya perabot (paket) sesuai keperluan penghuninya. Kamu sebagai penghuninya bisa masuk ke gedung sesuai pekerjaan, sehingga tidak tercampur dengan aktivitas di gedung lain.

Dengan mengikuti panduan ini, Anda sekarang memiliki:

- Anaconda terinstal di sistem
- UV environment siap digunakan
- Pengetahuan dasar manajemen environment

Selamat mencoba! 🚀
