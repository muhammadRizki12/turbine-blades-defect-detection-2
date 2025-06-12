# Turbine Blades Defect Detection

Proyek ini merupakan bagian dari **Capstone Project Program Laskar AI** yang berfokus pada deteksi cacat pada _turbine blade_, komponen penting dalam mesin turbin gas pesawat. Mengingat turbine blade bekerja dalam kondisi ekstrem (suhu tinggi, tekanan tinggi, dan kecepatan rotasi tinggi), deteksi dini terhadap kerusakan atau cacat sangat krusial untuk mencegah kegagalan mesin dan menjamin keselamatan operasional.

## Deskripsi

Kerusakan pada turbine blade dapat menyebabkan:

- Penurunan efisiensi mesin
- Biaya perawatan yang tinggi
- Potensi kerusakan mesin total
- Risiko keselamatan penerbangan

Tujuan dari proyek ini adalah membangun model machine learning yang mampu mendeteksi cacat pada turbine blade berdasarkan citra yang tersedia. Proyek ini terinspirasi dari paper:

> Zhang, Zilong, et al. (2023). _MMR: Multi-Modal Reasoning for Defect Detection_. [arXiv:2304.02216v2](https://arxiv.org/pdf/2304.02216v2)

Dataset yang digunakan berasal dari:

- [GitHub - MMR Dataset Repository](https://github.com/zhangzilongc/MMR)
- [Google Drive Dataset (zip)](https://drive.google.com/drive/folders/1CD2biD359dmvy81SDwsI26CA0mY9k3JM?usp=sharing)

---

## Struktur Direktori

- datasets/
- preprocessing.ipynb
- model.ipynb
- inference.ipynb
- requirements.txt
- README.md

---

## Instalasi

1. **Clone repositori:**

```bash
git clone https://github.com/muhammadRizki12/turbine-blades-defect-detection-2.git
```

2. Buat dan aktifkan environment Python:

```bash
conda create --name main-ds python=3.9
conda activate main-ds
pip install -r requirements.txt
```

3. Unduh dan ekstrak dataset:

   - Klik untuk download dataset - [Google Drive Dataset (zip)](https://drive.google.com/drive/folders/1CD2biD359dmvy81SDwsI26CA0mY9k3JM?usp=sharing)
   - Ekstrak dan simpan ke folder bernama datasets di root direktori proyek.

## Cara Penggunaan

1. Preprocessing data:

   Jalankan file preprocessing.ipynb untuk melakukan pembersihan, augmentasi, dan persiapan data sebelum pelatihan model.

2. Melatih model:

   Jalankan file model.ipynb untuk melakukan training dan evaluasi performa model pada dataset.

3. Inferensi / Prediksi:

   Gunakan file inference.ipynb untuk melakukan prediksi terhadap citra baru atau dataset uji.
