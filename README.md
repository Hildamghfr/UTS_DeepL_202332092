# UTS Deep Learning - Implementasi CNN dan Transfer Learning

Proyek ini dibuat untuk tugas UTS Deep Learning menggunakan dataset **MNIST** serta data tulisan tangan pribadi.  
Terdapat dua model yang dilatih:
- **Model A:** CNN sederhana (dibangun dari nol)
- **Model B:** Transfer Learning menggunakan **ResNet50**

##  Cara Menjalankan di Google Colab

### 1. Persiapan Awal
1. Buka [Google Colab](https://colab.research.google.com/).  
2. Klik **File → Upload notebook**.  
3. Unggah file: UTS_DeepL_A_202332092_Hilda Maghfira Genansi.py

> Alternatif: buat notebook baru, lalu salin seluruh isi kode dari file ini.

---

### 2. Instalasi Library
Google Colab biasanya sudah menyertakan semua library yang diperlukan.  
Namun jika ada error seperti `ModuleNotFoundError`, jalankan perintah berikut:

```bash
!pip install tensorflow opencv-python

```

### 3. Jalankan Kode
1. Jalankan setiap sel secara berurutan dari atas ke bawah tanpa melewatkan apa pun.
2. Program akan melakukan langkah-langkah berikut:
3. Memuat dan memproses dataset MNIST
4. Melatih dua model CNN (Model A dan Model B)
5. Menampilkan grafik akurasi dan loss
6. Melakukan validasi menggunakan data tulisan tangan dari folder uts

### 4. Persiapkan Folder Validasi
Buat folder bernama uts di direktori kerja Colab (/content/).
Isi folder dengan gambar angka tulisan tangan kamu menggunakan format:
nol_1.jpg, nol_2.jpg, ..., nol_10.jpg  
sembilan_1.jpg, ..., sembilan_10.jpg  
dua_1.jpg, ..., dua_10.jpg

Melalui upload langsung:
from google.colab import files
uploaded = files.upload()

### 5. Melihat Hasil
Setelah seluruh kode dijalankan, hasil yang akan muncul:
  - Grafik Training History: menunjukkan akurasi dan loss tiap epoch.
  - Evaluasi Model: menampilkan hasil uji akurasi pada dataset MNIST.
  - Validasi Tulisan Tangan: menampilkan grid gambar dengan prediksi model.

Warna judul pada tiap gambar menunjukkan hasil:
🟩 Hijau: prediksi benar
🟥 Merah: prediksi salah

