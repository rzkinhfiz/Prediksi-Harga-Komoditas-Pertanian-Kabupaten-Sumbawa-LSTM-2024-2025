# Prediksi Harga Komoditas Pertanian di Kabupaten Sumbawa menggunakan LSTM

Proyek ini merupakan implementasi riset skripsi yang berfokus pada prediksi harga komoditas pertanian di wilayah Kabupaten Sumbawa. Mengingat fluktuasi harga yang tinggi dan ketergantungan pada faktor geografis, penelitian ini menggunakan pendekatan *Deep Learning* (LSTM) untuk membantu stabilisasi ekonomi lokal dan deteksi dini perubahan harga.

## 📌 Deskripsi Proyek
Model ini dirancang untuk menangani data *time-series* harga pangan yang memiliki pola musiman. Proyek ini berhasil mengatasi tantangan infrastruktur data lokal dan keterbatasan referensi akademik spesifik wilayah, menghasilkan model dengan akurasi tinggi.

* **Algoritma:** Long Short-Term Memory (LSTM)
* **Wilayah Fokus:** Kabupaten Sumbawa, NTB, Indonesia
* **Deskripsi dataset:**
    - Dataset harga pasar tanaman pangan 2022-2024
    - Dataset Produktivitas tanaman pangan 2022-2023
 
## 📊 Visualisasi Hasil Prediksi
Hasil akhir prediksi dapat diakses melalui dashboard interaktif Looker Studio:

[Dashboard hasil prediksi harga pertanian](https://datastudio.google.com/s/pmrZrcKfXio)

## ⚡ Akselerasi GPU (RAPIDS & CUDA)
Proyek ini dioptimalkan menggunakan NVIDIA RAPIDS untuk mempercepat pemrosesan data dan pelatihan model pada hardware NVIDIA.

**Persyaratan Sistem:**
* **GPU:** NVIDIA Pascal™ atau lebih baru
* **Driver:** NVIDIA Driver v535.54.03+
* **CUDA:** Versi 12.x

### Instalasi Lingkungan (Conda)
Disarankan menggunakan `conda` untuk mengelola dependensi RAPIDS 24.10:

```bash
conda create -n modelpredict -c rapidsai -c conda-forge -c nvidia \
    rapids=24.10 python=3.10 cuda-version=12.5 \
    tensorflow-gpu pandas matplotlib scikit-learn
conda activate modelpredict
```

## 🛠️ Library yang Digunakan
**Bahasa Pemrograman:** Python
**Library Utama:**
* TensorFlow / Keras (Pembangunan model LSTM)
* Pandas & NumPy (Manipulasi data)
* Matplotlib / Seaborn (Visualisasi data)
* Scikit-learn (Preprocessing & Evaluasi)








