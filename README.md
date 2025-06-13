# 🚀 Setup Environment Data Science/AI (Anaconda • Conda • UV)
Nama : Almar Reza Maulana \
Batch : 9 \
No. Absen :9.050.DB2025 

Hallo semuanya ! Selamat datang di project saya yang lain. Disini saya akan membuat tutorial lingkungan kerja Data Science/AI. Di sini kita bakal belajar:

- Apa itu **Anaconda**, **Conda**, dan **UV**
- Cara install dan step-by-stepnya
- Do’s & Don’ts biar nggak salah langkah

## Pengenalan Anaconda, Conda , dan UV
➡️ Anaconda adalah distribusi Python yang super populer, dikembangin sama Anaconda, Inc. yang spesifik banget buat kebutuhan ilmu data dan analisis numerik. Dia dirancang untuk jadi "toolkit lengkap" bagi para ilmuwan data, biar semua yang kamu butuhin udah ada dalam satu paket. 😎🐍\
Apa aja sih isinya?\
Anaconda nggak hanya menyediain interpreter Python, tapi juga sejumlah pustaka keren seperti:
- NumPy & Pandas: Buat olah dan analisis data.
- Matplotlib: Buat visualisasi data yang kece.
- SciPy & Scikit-learn: Buat analisis numerik dan pembelajaran mesin.
Selain itu, ada juga alat-alat pendukung yang nggak kalah penting, kayak:
- Jupyter Notebook: Biar kamu bisa interaktif coding dan coba-coba langsung.
- Spyder: IDE buat coding Python yang nyaman.
- Anaconda Navigator: GUI yang bikin kamu bisa ngatur environment dan install paket lewat klik-klik, tanpa harus repot dengan command line. 🚀💻
  
➡️ Conda adalah tool open source dari Anaconda yang mengelola paket dan virtual environment. Dengan conda, kamu bisa instal, update, atau hapus paket beserta dependency-nya dan membuat lingkungan kerja terpisah untuk setiap proyek sehingga tidak terjadi bentrok. Karena paketnya precompiled, instalasinya jadi mudah tanpa harus membangun dari source. Selain Python, conda juga mendukung bahasa lain.

➡️ UV dalam Python , yaitu fitur yang memungkinkan kamu membuat lingkungan kerja terpisah untuk setiap proyek. Dengan virtual environment, setiap proyek punya versi Python dan paketnya sendiri, sehingga tidak bentrok dengan proyek lain. Ini berguna banget buat manajemen dependency dan menjaga sistem tetap bersih tanpa harus install paket secara global. 🚀🐍


## 📥 CHAPTER 1 : Anaconda & Conda
Anaconda dan Conda itu mirip tapi punya peran yang beda \
✔ Anaconda adalah distribusi Python yang udah satu paket dengan banyak library untuk Data Science dan AI. Jadi, kalau kamu install Anaconda, udah otomatis dapat Python, Conda, Jupyter Notebook, pandas, NumPy, dll.\
✔ Conda adalah package & environment manager yang ada di dalam Anaconda. Tapi, kamu bisa pakai Conda secara terpisah lewat Miniconda. Conda ini berguna buat mengatur virtual environment dan install paket tanpa ribet.

Apa : Anaconda merupakan distribusi Python yang populer, yang dirancang untuk ilmu data, pembelajaran mesin, dan analisis data.\
Kenapa : Anaconda memungkinkan kita untuk membuat dan mengelola lingkungan terpisah untuk proyek yang berbeda

## 🪜 Tahapan unduh dan instalasi anaconda

➤ Langkah 1: Kunjungi Situs Resmi Anaconda
![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-12%20082404.png)
Kunjungi situs download resmi Anaconda: https://www.anaconda.com/download

-Do : download installer di website anaconda resmi yah \
-Don't : Hindari link download dari blog tidak resmi, forum, atau situs berbagi file. Hanya gunakan situs resmi Anaconda.\

➤ Langkah 2: Pilih Installer yang Sesuai
Pilih salah satu sistem operasi yang kamu pakai (Windows, macOS, atau Linux). lalu
pilih installer 64-Bit Graphical Installer.

➤ Langkah 3: Download File Installer
Klik tombol Download.
Browser akan mulai mengunduh file installer (misalnya, Anaconda3-2023.09-0-Windows-x86_64.exe). Tunggu hingga proses download selesai.

➤ Langkah 4: Jalankan File Installer
Buka folder "Downloads" di komputer Anda.
Cari file installer yang baru saja diunduh.
Klik dua kali pada file tersebut untuk memulai proses instalasi. Jika muncul peringatan keamanan dari Windows, klik "Run" atau "Yes".

➤ Langkah 5: Ikuti Petunjuk Instalasi (Installation Wizard)
Ini adalah bagian paling krusial. Baca setiap langkah dengan teliti.
1. Welcome Screen: Klik "Next" untuk memulai.\
  ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-12%20092026.png) 
3. License Agreement (Perjanjian Lisensi): Klik "I Agree" untuk melanjutkan.
4. Select Installation Type (Pilih Tipe Instalasi)🏠︎:\
 ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20092640.png)\
• Kamu akan diberi dua pilihan: "Just Me" atau "All Users".\
• Pilih aja "Just Me". Opsi ini lebih sederhana, tidak memerlukan hak administrator, dan menghindari banyak potensi masalah perizinan di kemudian hari.\
• Klik "Next".
5. Choose Install Location (Pilih Lokasi Instalasi)📍: \
 ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20094755.png)\
• Disarankan untuk membiarkan lokasi instalasi di folder default yang disarankan oleh installer (biasanya di C:\Users\Nama_Kamu\anaconda3).\
• PENTING: Jangan memilih folder yang namanya mengandung spasi atau karakter non-latin (seperti C:\Program Files\Anaconda). Ini bisa menyebabkan masalah saat menjalankan program dari command line.\
• Klik "Next".
7. Advanced Installation Options (Opsi Instalasi Lanjutan)✔️: \
 ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-12%20092711.png)\
Centang 3 kotak ini. Ini buat mastiin bahwa aplikasi yang membutuhkan Python akan mengenali Python dari Anaconda. Setelah selesai, klik "Install".
8. Installation Progress (Proses Instalasi)⏳:
Proses instalasi akan dimulai. Setelah instalasi selesai, klik "Next". Kamu mungkin akan melihat layar tentang "Anaconda Distribution". Klik "Next" lagi. lalu pada layar terakhir kamu bisa langsung klik "Finish".

➤ Langkah 6 : Cek Instalasi Anaconda kamu 🧐 \
![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20101242.png)\
Untuk memastikan Anaconda kamu sudah terinstall dengan benar di sistem kamu, bisa lakukan verifikasi lewat Command Prompt (CMD) lalu ketik ```conda -- version```

➤ Langkah 7 : Konfigurasi Variabel Lingkungan Path 🔗
Nah, biar gak ribet tiap kali mau panggil conda atau python dari Anaconda, kamu bisa set PATH Environment Variable biar bisa dipanggil dari terminal manapun tanpa harus buka Anaconda Navigator dulu. Caranya :
1. Buka Pengaturan path :\
 - Tekan Win + S, cari "Edit system environment variables" lalu klik "Environment Variable" .
2. Tambahkan Path Baru
 - Klik Edit Variables di bagian "System Variables" → cari Path → klik Edit → tambah path berikut:
   ```
   C:\Users\Nama_user\anaconda3
   C:\Users\Nama_user\anaconda3\Library\mingw-w64\bin
   C:\Users\Nama_user\anaconda3\Library\usr\bin
   C:\Users\Nama_user\anaconda3\Library\bin
   C:\Users\Nama_user\anaconda3\Scripts
   ```
![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20105139.png)
   
➤ Langkah 8 : Membuat environment conda yang baru 🏡

Kenapa kita harus buat environment yang baru? karena kita mau project yang kita buat lebih tertata rapi dan tercampur aduk dengan yang lain. Untuk melakukannya kita bisa :
Buka terminal kembali → Jalankan perintah ini: conda create -n nama_env python=3.9 → klik y \
![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20110412.png)


## CHAPTER 2 : Membuat UV Environmnet 
Kenapa kita harus buat UV? karena UV biar tiap proyek punya ruang kerja sendiri tanpa campur-aduk paket. Caranya gampang kok! Teman-teman bisa ikutin langkah-langkah ini:\
✈︎ Langkah 1 : Buat UV baru 

Buka terminal → ketik perintah ini : pip install uv \
![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20120714.png)

Do : Beri nama environment yang deskriptif \
Don't: Jangan gunakan environment base untuk proyek
  
✈︎ Langkah 2 : Menginisialisasi proyek UV

🔹 Apa Itu Inisialisasi Proyek UV?
Ini adalah proses bikin struktur proyek dan set virtual environment supaya semua paket dan versi Python terpisah dari proyek lain. Jadi proyek lo rapi, aman, dan gak kena konflik dependency!\
🔹 Kenapa Harus Diinisialisasi?\
✔ Biar teratur: Setiap proyek punya lingkungan sendiri tanpa ganggu sistem utama 🏗️\
✔ Bebas dari konflik: Paket versi lama vs baru gak akan saling tabrakan 💥\
Cara melakukan inisialisasi UV dengan cara berikut :
1. Buka terminal
2. Ketik Perintah ini : uv init ghost_intellixuv setelah itu Cd ghost_intellixuv
3. Output proyek yang udah diinisialisasi tulisannya bakal seperti ini  di C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv. \
   ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20123716.png) 

🔥 Do’s & Don’ts Pas Inisialisasi UV\
✅ Do’s: \
✔ Gunakan nama environment yang jelas & intuitif biar gampang diingat. \
✔ Simpan requirements.txt buat dokumentasi paket proyek. \
✔ Selalu aktifkan env sebelum mulai coding biar paketnya gak terinstal di sistem utama.

❌ Don’ts: \
✖ Jangan bikin environment di dalam proyek lain, nanti kacau balau! 🤯 \
✖ Jangan lupa deactivate kalau udah selesai biar terminal bersih.

✈︎ Langkah 3 : Membuat dan Mengaktifkan Lingkungan UV\

untuk buat dan aktifin lingkungan UV kamu bisa ikuti langkah ini :
1. buka terminal tadi dan ketik perintah ini  : ```uv venv```
2. jika sudah dibuat lingkungan UV nya, kamu bisa aktifin dengan ketik perintah ini : ```.venv\Scripts\activate```
3. Hasilnya Prompt berubah ke (ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>. \
  ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20125509.png)

✅ Do : Gunakan environment yang tadi sudah dibuat di langkah 2 chapter 2 \
❌ Don’t: Jangan bikin environment di dalam proyek lain

✈︎ Langkah 4 : Menginstall Paket dengan UV\

Karena kita sudah bikin UV dan udah tau juga aktifinnya. Sekarang kita lanjut install paket ini biar proyek nya makin power up soalnya dengan paki UV ini kita bisa menghemat waktu daripada menginstall seperti biasanya! \
✅ Do: Gunakan uv add.\
❌ Don't: Jangan campur UV dan pip.\
Caranya  yaitu :
1. buka terminal seperti biasanya
2. ketik perintah ini :```uv add pandas```
3. Output dari perintah tadi hasilnya akan seperti di bawah ini : \
   ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20125549.png)
   
✈︎ Langkah 5 : Menonaktifkan lingkungan UV\

Karena sebelumnya kita masih aktifin lingkungan UV nya, nah sekarang kita nonaktifkan supaya sistem utama python kita bersih dan gak ada yang nyasar pas saat ngerjain proyek diluar UV. Caranya gampang banget teman-teman bisa langsung aja ketik perintah ini di terminal kamu : ```.venv\Scripts\deactivate```. Setelah itu selesai UV udah otomatis nonaktif 

## Chapter 3 : Manajemen Environment 
Manajemen proyek ini dibuat agar teman-teman langsung satset ketika ingin cepat membuat ataupun mengelola sebuah proyek. \
 ![TASK-SETUP-ANACONDA-UV](https://github.com/Almar-Reza-Maulana/TASK-SETUP-ANACONDA-UV/blob/main/SS/Screenshot%202025-06-13%20140751.png)

 ## 🚀 Penutup
Dengan memahami cara setup environment menggunakan Anaconda, Conda, dan UV, kita bisa memastikan proyek Data Science/AI tetap rapi, terisolasi, dan bebas konflik dependency.
Manajemen environment bukan cuma soal menghindari error, tapi juga soal efisiensi dan fleksibilitas dalam mengelola proyek. Dengan langkah-langkah yang sudah dibahas di repository ini, kita bisa lebih mudah menyiapkan lingkungan kerja yang stabil dan siap untuk eksplorasi lebih lanjut. Terima Kasih sudah melihat repository ini 😊


