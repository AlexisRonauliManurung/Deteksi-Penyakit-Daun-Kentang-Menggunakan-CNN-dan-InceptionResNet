# Deteksi Penyakit Daun Kentang Menggunakan CNN dan InceptionResNet

Proyek ini dibuat untuk memenuhi tugas Ujian Tengah Semester (UTS) mata kuliah Computer Vision. Tujuannya adalah untuk membangun model *deep learning* yang dapat mendeteksi dan mengklasifikasikan penyakit pada daun kentang.

## 📝 Deskripsi

Notebook ini mengimplementasikan dua arsitektur *Convolutional Neural Network* (CNN) untuk mengklasifikasikan tiga kondisi daun kentang: **Early Blight**, **Late Blight**, dan **Healthy** (Sehat). Dua model yang digunakan adalah:

1.  Model CNN sederhana yang dibangun dari awal.
2.  Model *transfer learning* menggunakan arsitektur **InceptionResNetV2**.

Tujuannya adalah untuk membandingkan performa kedua model dalam mendeteksi penyakit daun kentang secara akurat.

## 📊 Dataset

Dataset yang digunakan dalam proyek ini adalah **Potato Disease Leaf Dataset** yang tersedia di Kaggle.

  * **Sumber:** [rizwan123456789/potato-disease-leaf-datasetpld](https://www.kaggle.com/datasets/rizwan123456789/potato-disease-leaf-datasetpld)
  * **Kelas:** Dataset ini memiliki tiga kelas citra daun kentang:
    1.  `Early_Blight`
    2.  `Late_Blight`
    3.  `Healthy`

## ⚙️ Kebutuhan Pustaka (Libraries)

Pastikan Anda telah menginstal pustaka Python berikut sebelum menjalankan notebook:

```
numpy
pandas
matplotlib
tensorflow
kagglehub
```

Anda dapat menginstalnya menggunakan pip:
`pip install numpy pandas matplotlib tensorflow kagglehub`

## 🚀 Cara Menjalankan

1.  **Unduh Notebook**: Simpan file `Deteksi_Penyakit_Daun_Kentang_Menggunakan_CNN_dan_InceptionResNet.ipynb` di direktori kerja Anda.
2.  **Instal Pustaka**: Pastikan semua pustaka yang tercantum di atas sudah terinstal.
3.  **Jalankan Jupyter Notebook**: Buka dan jalankan sel-sel kode di dalam notebook secara berurutan. Notebook ini akan secara otomatis mengunduh dataset dari Kaggle menggunakan pustaka `kagglehub`.
4.  **Proses**: Notebook akan melalui langkah-langkah berikut:
      * Mengimpor dataset dari Kaggle.
      * Memuat dan melakukan pra-pemrosesan data citra.
      * Membangun, melatih, dan mengevaluasi kedua model (CNN dan InceptionResNetV2).
      * Menampilkan visualisasi citra dan (jika ada) plot hasil pelatihan.

## 🤖 Arsitektur Model

### 1\. CNN Sederhana

Model ini terdiri dari beberapa lapisan konvolusi (`Conv2D`) dan *pooling* (`MaxPooling2D`) yang diikuti oleh lapisan *fully connected* (`Dense`) untuk klasifikasi.

### 2\. InceptionResNetV2

Model ini menggunakan pendekatan *transfer learning* dengan memanfaatkan arsitektur InceptionResNetV2 yang sudah dilatih sebelumnya pada dataset ImageNet. Lapisan-lapisan atasnya disesuaikan untuk tugas klasifikasi penyakit daun kentang ini.

## 👨‍💻 Kontributor

  * **Nama:** Alexis Ronauli Manurung
  * **NIM:** 2215061109
