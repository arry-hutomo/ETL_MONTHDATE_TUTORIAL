# Panduan Lengkap Setup Anaconda & UV Environment untuk Data Science/AI
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

## Panduan Setup (Conda dan UV Virtual Environments).html 📑

## **Instalasi Anaconda**

### **1. Mengunduh Anaconda**

**Apa:** Anaconda adalah distribusi Python yang menyertakan ratusan paket siap pakai, ideal untuk analisis data dan komputasi ilmiah.

**Kenapa:** Mengunduh Anaconda memberikan akses ke alat-alat penting untuk Data Science tanpa instalasi paket manual. Ini memastikan kompatibilitas dan menghemat waktu.

**Do and Don'ts:**

- **Do:** Pilih Python 3.12 untuk kompatibilitas maksimal.
- **Don't:** Hindari versi 32-bit kecuali perangkat Anda tidak mendukung 64-bit.
  
**Langkah-langkah:**

1. Kunjungi **https://www.anaconda.com/download.**
2. Pilih penginstal: **Windows Python 3.12 64-Bit Graphical Installer (921.3MB).**
3. **Simpan file di Desktop** atau folder Unduhan.

### **2. Proses Instalasi**

**Apa:** Instalasi melibatkan menjalankan file penginstal dan mengatur konfigurasi sistem.

**Kenapa:** Instalasi yang benar memungkinkan Anaconda terintegrasi dengan sistem, sehingga perintah Conda dan Python dapat diakses dari terminal.

**Do and Don'ts:**

- **Do:** Centang opsi untuk menambahkan Anaconda ke PATH.
- **Don't:** Jangan ubah lokasi instalasi default tanpa alasan kuat.

**Langkah-langkah:**

1. Klik dua kali **Anaconda3-2024.10-1-Windows-x86_64.exe**.



2. Klik **"Next"** pada layar sambutan.
   
   ![alt text](image/conda1.png)
   
3. Setujui syarat lisensi **(I Agree)**.

   ![alt text](image/conda2.png)
   
4. Pilih **"Just Me (recommended)"**.

   ![alt text](image/conda3.png)
   
5. Gunakan lokasi **default** (C:\Users\NAMA_ANDA\anaconda3).

   ![alt text](image/conda4.png)
   
6. Pilih **Checklist**:

   ✓ Tambahkan Shortcut.
 
   ✓ Tambahkan Anaconda3 ke PATH.
  
   ✓ Jadikan Anaconda3 sebagai Python 3.12 default.
  
   ![alt text](image/conda5.png)
  
9. Klik **"Install"** dan tunggu **Finish**.

   ![alt text](image/conda6.png)

   ![alt text](image/conda7.png)

   ![alt text](image/conda8.png)

   ![alt text](image/conda9.png)
   
**Peringatan:** Jika lupa mencentang "Tambahkan ke PATH", Anda harus mengatur PATH secara manual.

### 3. Verifikasi

**Apa:** Verifikasi memastikan Anaconda terinstal dan dapat diakses.

**Kenapa:** Ini mendeteksi masalah seperti PATH yang salah, memungkinkan perbaikan dini.

**Do and Don'ts:**

**Do:** Buka terminal baru untuk menerapkan perubahan PATH.
**Don't:** Jangan abaikan pesan kesalahan.

**Langkah-langkah:**

1. Buka **Command Prompt**.
2. Ketik dan eksekusi:
   **conda --version**

![alt text](image/conda10.png)

Output seperti **conda 24.9.2** menunjukkan keberhasilan.




