# ETL_MONTHDATE_TUTORIAL (001)
Panduan lengkap untuk setup lingkungan Python dengan Anaconda &amp; UV. Anaconda menyediakan ratusan paket siap pakai untuk komputasi ilmiah &amp; analisis data, sementara UV adalah alat manajemen paket berbasis Rust yang cepat untuk lingkungan virtual &amp; instalasi dependensi. Cocok untuk pemula dalam proyek AI/ML. 🚀
![CONDAUV](https://github.com/arry-hutomo/ETL_MONTHDATE_TUTORIAL/blob/main/CONDA%20UV%20ENVIRONMENTs.png)

### 🌱 Latar Belakang Pentingnya dalam Proyek AI dan ML

##### Lingkungan virtual seperti yang disediakan oleh Anaconda dan UV sangat krusial dalam proyek Artificial Intelligence (AI) dan Machine Learning (ML). Mengapa? Proyek AI/ML sering kali memerlukan berbagai pustaka dan versi Python yang berbeda, seperti TensorFlow, PyTorch, atau scikit-learn, yang dapat bertabrakan jika tidak dikelola dengan baik. Dengan lingkungan terisolasi, Anda dapat:





Menghindari konflik versi antar paket. ✅



Memastikan konsistensi dan reproduktibilitas hasil. 🔄



Mengelola dependensi secara efisien, terutama pada proyek kompleks. ⚙️
Pengaturan ini memungkinkan pengembang fokus pada pengembangan model tanpa khawatir masalah teknis lingkungan, sehingga meningkatkan produktivitas dan kualitas proyek. ⏳

🛠️ Cara Penggunaan

Silakan ikuti panduan terperinci yang terdapat dalam file utama:


---

### Panduan Setup (Conda dan UV Virtual Environments).html 📑

 ####Instalasi Anaconda
#####1.1 Mengunduh Anaconda
Apa: Anaconda adalah distribusi Python yang menyertakan ratusan paket siap pakai, ideal untuk analisis data dan komputasi ilmiah.

Kenapa: Mengunduh Anaconda memberikan akses ke alat-alat penting untuk Data Science tanpa instalasi paket manual. Ini memastikan kompatibilitas dan menghemat waktu.

Do and Don'ts:

Do: Pilih Python 3.12 untuk kompatibilitas maksimal.
Don't: Hindari versi 32-bit kecuali perangkat Anda tidak mendukung 64-bit.
Langkah-langkah:

Kunjungi https://www.anaconda.com/download.
Pilih penginstal: Windows Python 3.12 64-Bit Graphical Installer (921.3MB).
Simpan file di Desktop atau folder Unduhan.
#####1.2 Proses Instalasi
Apa: Instalasi melibatkan menjalankan file penginstal dan mengatur konfigurasi sistem.

Kenapa: Instalasi yang benar memungkinkan Anaconda terintegrasi dengan sistem, sehingga perintah Conda dan Python dapat diakses dari terminal.

Do and Don'ts:

Do: Centang opsi untuk menambahkan Anaconda ke PATH.
Don't: Jangan ubah lokasi instalasi default tanpa alasan kuat.
Langkah-langkah:

Klik dua kali Anaconda3-2024.10-1-Windows-x86_64.exe.
Klik "Next" pada layar sambutan.
Setujui syarat lisensi.
Pilih "Just Me (recommended)".
Gunakan lokasi default (C:\Users\NAMA_ANDA\anaconda3).
Centang:
✓ Tambahkan Anaconda3 ke PATH.
✓ Jadikan Anaconda3 sebagai Python 3.12 default.
Klik "Install" dan tunggu selesai.
Peringatan: Jika lupa mencentang "Tambahkan ke PATH", Anda harus mengatur PATH secara manual.
#####1.3 Verifikasi
Apa: Verifikasi memastikan Anaconda terinstal dan dapat diakses.

Kenapa: Ini mendeteksi masalah seperti PATH yang salah, memungkinkan perbaikan dini.

Do and Don'ts:

Do: Buka terminal baru untuk menerapkan perubahan PATH.
Don't: Jangan abaikan pesan kesalahan.
Langkah-langkah:

Buka Command Prompt.
Ketik dan eksekusi:
conda --version
Output seperti conda 24.1.0 menunjukkan keberhasilan.
Keberhasilan: Nomor versi mengonfirmasi instalasi berhasil.



