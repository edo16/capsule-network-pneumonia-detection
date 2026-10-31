# Implementasi Capsule Network untuk Deteksi Pneumonia

**Language:** Bahasa Indonesia | [English](./README_ENG.md)

## Deskripsi Proyek

Proyek ini merupakan implementasi model Capsule Network (CapsNet) dengan fungsi aktivasi untuk klasifikasi citra X-ray dalam mendeteksi pneumonia.

Penelitian ini bertujuan menerapkan metode Deep Learning untuk mengklasifikasikan citra rontgen dada ke dalam dua kategori, yaitu Normal dan Pneumonia.

Proyek ini merupakan bagian dari penelitian skripsi sebagai salah satu persyaratan penyelesaian pendidikan Sarjana Matematika.

## Tujuan Penelitian

1. Mengimplementasikan arsitektur Capsule Network untuk klasifikasi citra X-ray.
2. Menerapkan fungsi aktivasi pada arsitektur Capsule Network.
3. Melakukan pelatihan model menggunakan dataset citra X-ray.
4. Mengevaluasi kemampuan model dalam mengklasifikasikan citra Normal dan Pneumonia.
5. Menganalisis performa model berdasarkan metrik evaluasi klasifikasi.

## Dataset

Penelitian menggunakan dataset Chest X-Ray Images (Pneumonia) dari Kaggle yang disediakan oleh Paul Mooney.

Dataset terdiri dari 5.863 citra dengan dua kategori:

- Normal
- Pneumonia

### Pembagian Dataset

| Dataset | Jumlah Citra |
|---|---:|
| Pelatihan | 4.099 |
| Validasi | 877 |
| Pengujian | 880 |
| **Total** | **5.863** |

## Metodologi

Tahapan penelitian meliputi:

1. Pengumpulan dan persiapan dataset.
2. Pra-pemrosesan citra.
3. Pembagian dataset.
4. Pembangunan arsitektur Capsule Network.
5. Pelatihan model.
6. Validasi model.
7. Evaluasi performa model.

## Arsitektur Model

Komponen utama model:

- Convolutional Layer
- Primary Capsule Layer
- Digit Capsule Layer
- Dynamic Routing
- Squash Activation Function
- Margin Loss

## Konfigurasi Model

| Parameter | Nilai |
|---|---|
| Bahasa Pemrograman | Python |
| Framework | TensorFlow/Keras |
| Ukuran Citra | 128 × 128 piksel |
| Mode Warna | Grayscale |
| Epoch | 30 |
| Batch Size | 16 |
| Dimensi Primary Capsule | 8 |
| Dimensi Digit Capsule | 16 |
| Optimizer | Adam |
| Learning Rate | 0,0001 |
| Routing Iterations | 3 |
| Margin Positif (m+) | 0,9 |
| Margin Negatif (m-) | 0,1 |
| Lambda | 0,5 |

## Hasil Penelitian

| Metrik | Hasil |
|---|---:|
| Akurasi Pelatihan | 98,13% |
| Akurasi Validasi | 96,12% |
| Akurasi Pengujian | 96,36% |
| Loss Pengujian | 4,33% |

Model berhasil mengklasifikasikan 848 dari 880 citra pengujian dengan benar.

Evaluasi dilakukan menggunakan:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Classification Report

| Kelas | Precision | Recall | F1-Score | Support |
|---|---:|---:|---:|---:|
| Normal | 0,93 | 0,94 | 0,93 | 238 |
| Pneumonia | 0,98 | 0,97 | 0,97 | 642 |

## Teknologi yang Digunakan

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Struktur Repository

```text
capsule-network-pneumonia-detection/
├── notebooks/
│   └── capsule_network_pneumonia.ipynb
├── results/
├── thesis/
├── README.md
├── requirements.txt
└── LICENSE
```

## Dokumentasi Penelitian

**Judul Skripsi:**

Implementasi Model Capsule Network Dengan Fungsi Aktivasi Untuk Klasifikasi Citra X-ray Dalam Deteksi Pneumonia.

**Penulis:** Alfredo Raul Adamsyah

**Program Studi:** S1 Matematika

**Peminatan:** Statistika

**Universitas:** Universitas Lampung

## Catatan

Proyek ini dikembangkan untuk keperluan akademik dan penelitian. Model merupakan sistem klasifikasi citra eksperimental dan bukan pengganti diagnosis medis profesional.

Dataset tidak disertakan dalam repository. Pengguna perlu mengunduh dataset dari sumber Kaggle secara terpisah.

## Tentang Penulis

**Alfredo Raul Adamsyah**

Sarjana Matematika – Peminatan Statistika  
Universitas Lampung

Bidang Minat:

- Analisis Data
- Statistika
- Machine Learning
- Deep Learning
