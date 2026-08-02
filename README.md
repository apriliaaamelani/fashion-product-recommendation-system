# 👗 Fashion Product Recommendation System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Recommendation%20System-success" />
  <img src="https://img.shields.io/badge/Content--Based-TF--IDF-orange" />
  <img src="https://img.shields.io/badge/Collaborative-SVD-red" />
  <img src="https://img.shields.io/badge/Scikit--Learn-Latest-F7931E?logo=scikitlearn" />
  <img src="https://img.shields.io/badge/Surprise-Recommendation-blueviolet" />
</p>

---

## 📖 Overview

Perkembangan industri **e-commerce fashion** menyebabkan jumlah produk yang tersedia semakin banyak, sehingga pelanggan sering mengalami kesulitan menemukan produk yang sesuai dengan preferensi mereka. Oleh karena itu, sistem rekomendasi menjadi salah satu komponen penting dalam meningkatkan pengalaman pengguna serta membantu meningkatkan penjualan.

Proyek ini membangun **Fashion Product Recommendation System** menggunakan dua pendekatan utama:

- **Content-Based Filtering**, yang merekomendasikan produk berdasarkan kemiripan atribut produk.
- **Collaborative Filtering**, yang merekomendasikan produk berdasarkan pola preferensi pengguna lain menggunakan algoritma **Singular Value Decomposition (SVD)**.

Dataset yang digunakan berasal dari **Kaggle Fashion Products Dataset** dan berisi informasi mengenai produk, kategori, merek, warna, ukuran, harga, serta rating pengguna.

---

## 🎯 Project Objectives

Project ini bertujuan untuk:

- Mengembangkan sistem rekomendasi produk fashion menggunakan pendekatan Machine Learning.
- Membangun rekomendasi berbasis atribut produk (Content-Based Filtering).
- Membangun rekomendasi berbasis preferensi pengguna (Collaborative Filtering).
- Membandingkan dua metode rekomendasi yang berbeda.
- Mengevaluasi performa masing-masing metode menggunakan metrik yang sesuai.

---

# ✨ Features

Repository ini mengimplementasikan beberapa fitur utama, antara lain:

✅ Data preprocessing

✅ Feature Engineering

✅ TF-IDF Vectorization

✅ Cosine Similarity

✅ Content-Based Recommendation

✅ Collaborative Filtering (SVD)

✅ Top-N Recommendation

✅ Model Evaluation

---

# 🏗 Project Architecture

```text
                    Fashion Products Dataset
                              │
                              ▼
                     Data Preprocessing
                              │
              ┌───────────────┴───────────────┐
              │                               │
              ▼                               ▼
     Content-Based Filtering         Collaborative Filtering
              │                               │
     Combine Product Features         User-Item Rating Matrix
              │                               │
        TF-IDF Vectorizer                 Surprise Dataset
              │                               │
      Cosine Similarity                    SVD Model
              │                               │
              └───────────────┬───────────────┘
                              ▼
                 Top-N Product Recommendation
```

---

# 📂 Repository Structure

```text
fashion-product-recommendation-system
│
├── README.md
├── recommendation_system.py
├── recommendation_system.ipynb
│
├── dataset/
│   └── fashion_products.csv
```

# 🛠 Technology Stack

Project ini dibangun menggunakan teknologi berikut.

| Category | Technology |
|----------|------------|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-Learn |
| Recommendation System | Surprise (SVD) |
| Text Processing | TF-IDF Vectorizer |
| Similarity Measurement | Cosine Similarity |
| Visualization | Matplotlib, Seaborn |
| Notebook | Jupyter Notebook |

---

# 📦 Libraries

Beberapa library utama yang digunakan pada project ini meliputi:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- scikit-surprise
- TfidfVectorizer
- Cosine Similarity

---

# 🚀 Skills Demonstrated

Melalui project ini, beberapa kompetensi yang ditunjukkan antara lain:

- Machine Learning
- Recommendation System
- Feature Engineering
- Natural Language Processing (TF-IDF)
- Collaborative Filtering
- Content-Based Filtering
- Cosine Similarity
- Model Evaluation
- Data Visualization
- Data Preprocessing
---

# 📊 Dataset

Dataset yang digunakan dalam proyek ini adalah **Fashion Products Dataset** yang tersedia secara publik di Kaggle.

**Dataset Source**

https://www.kaggle.com/datasets/bhanupratapbiswas/fashion-products

Dataset terdiri dari **1.000 data produk fashion** dengan **9 atribut**, meliputi informasi produk dan interaksi pengguna.

| Feature | Description |
|----------|-------------|
| User ID | ID pengguna |
| Product ID | ID produk |
| Product Name | Nama produk |
| Brand | Merek produk |
| Category | Kategori fashion |
| Price | Harga produk |
| Rating | Rating yang diberikan pengguna |
| Color | Warna produk |
| Size | Ukuran produk |

Dataset ini tidak memiliki missing value maupun data duplikat sehingga dapat langsung digunakan untuk proses pengembangan model.

---

# 🎯 Business Understanding

## Background

Pada platform e-commerce, pengguna dihadapkan pada ribuan bahkan jutaan produk. Tanpa sistem rekomendasi yang baik, pengguna akan kesulitan menemukan produk yang sesuai dengan preferensi mereka.

Sistem rekomendasi membantu pengguna menemukan produk yang relevan berdasarkan karakteristik produk maupun perilaku pengguna lainnya.

---

## Problem Statement

Permasalahan yang ingin diselesaikan pada proyek ini adalah:

- Bagaimana memberikan rekomendasi produk fashion yang relevan berdasarkan karakteristik produk?
- Bagaimana memberikan rekomendasi berdasarkan preferensi pengguna lain yang memiliki pola perilaku serupa?
- Bagaimana membandingkan performa Content-Based Filtering dan Collaborative Filtering?

---

## Objectives

Proyek ini memiliki beberapa tujuan utama.

- Mengembangkan sistem rekomendasi berbasis atribut produk.
- Mengembangkan sistem rekomendasi berbasis interaksi pengguna.
- Membandingkan performa kedua metode rekomendasi.
- Menghasilkan rekomendasi produk yang relevan.

---

# 🔍 Data Understanding

Sebelum membangun model, dilakukan eksplorasi terhadap dataset.

## Jumlah Data

- Total Data : **1000**
- Total Features : **9**

---

## Missing Value

Tidak ditemukan missing value pada dataset.

```
Missing Value : 0
```

---

## Duplicate Data

Tidak ditemukan data duplikat.

```
Duplicate Data : 0
```

---

## Product Categories

Dataset terdiri dari berbagai atribut produk seperti:

- Product Name
- Brand
- Category
- Color
- Size

Atribut-atribut tersebut digunakan sebagai representasi karakteristik produk pada metode Content-Based Filtering.

---

## User Interaction

Untuk metode Collaborative Filtering digunakan tiga atribut utama.

- User ID
- Product ID
- Rating

Ketiga atribut tersebut digunakan untuk membangun User-Item Interaction Matrix menggunakan library Surprise.

---

# ⚙ Data Preparation

Tahapan data preparation dilakukan sebelum proses pemodelan.

## 1. Feature Engineering

Beberapa atribut produk digabungkan menjadi satu kolom baru.

```
Product Name
Brand
Category
Color
Size
```

menjadi

```
combined_features
```

Tujuannya adalah agar seluruh informasi produk dapat direpresentasikan dalam satu dokumen teks sebelum dilakukan proses TF-IDF.

---

## 2. TF-IDF Vectorization

Kolom `combined_features` kemudian diproses menggunakan **TF-IDF Vectorizer**.

TF-IDF mengubah data teks menjadi representasi numerik sehingga dapat dihitung tingkat kemiripan antar produk.

Output tahap ini berupa matriks TF-IDF.

---

## 3. Cosine Similarity Matrix

Matriks TF-IDF digunakan untuk menghitung **Cosine Similarity** antar produk.

Semakin tinggi nilai similarity, semakin mirip karakteristik kedua produk tersebut.

Hasil similarity inilah yang digunakan pada Content-Based Filtering.

---

## 4. Collaborative Filtering Dataset

Untuk metode Collaborative Filtering digunakan data:

- User ID
- Product ID
- Rating

Data kemudian dikonversi menggunakan **Reader** dan **Dataset.load_from_df()** dari library Surprise.

---

## 5. Train-Test Split

Data interaksi pengguna dibagi menjadi:

- Training Set
- Testing Set

Pembagian ini digunakan agar model dapat dievaluasi menggunakan data yang belum pernah dilihat sebelumnya.

---

# 🧠 Content-Based Filtering

Metode pertama yang digunakan adalah **Content-Based Filtering**.

Metode ini memberikan rekomendasi berdasarkan kemiripan karakteristik produk.

Tahapan yang dilakukan yaitu:

```
Product Features
        │
        ▼
Combine Features
        │
        ▼
TF-IDF
        │
        ▼
Cosine Similarity
        │
        ▼
Top-N Recommendation
```

Produk yang memiliki nilai cosine similarity tertinggi akan direkomendasikan kepada pengguna.

---

## Example Recommendation

Sebagai contoh digunakan:

```
Product ID : 1
```

Top-10 rekomendasi yang dihasilkan antara lain:

| Product ID | Product | Brand | Category |
|------------|----------|--------|----------------|
| 829 | Dress | Adidas | Men's Fashion |
| 489 | Dress | Adidas | Men's Fashion |
| 756 | Jeans | Adidas | Men's Fashion |
| 240 | Dress | H&M | Men's Fashion |
| 678 | Dress | H&M | Men's Fashion |
| 761 | Dress | H&M | Men's Fashion |
| 441 | Sweater | Adidas | Men's Fashion |
| 459 | Dress | Adidas | Kids' Fashion |
| 295 | Dress | H&M | Kids' Fashion |
| 209 | Dress | H&M | Women's Fashion |

---

# 👥 Collaborative Filtering

Metode kedua menggunakan **Collaborative Filtering**.

Model dibangun menggunakan algoritma **Singular Value Decomposition (SVD)** dari library Surprise.

Tahapan prosesnya adalah:

```
User Rating
      │
      ▼
Dataset Surprise
      │
      ▼
SVD Training
      │
      ▼
Rating Prediction
      │
      ▼
Top-N Recommendation
```

Model mempelajari pola interaksi pengguna untuk memprediksi rating produk yang belum pernah diberikan.

---

## Example Recommendation

Contoh pengguna:

```
User ID : 19
```

Top-10 rekomendasi yang dihasilkan.

| Product ID | Product | Brand | Category |
|------------|----------|--------|----------------|
| 10 | T-shirt | Zara | Kids' Fashion |
| 26 | Dress | Gucci | Women's Fashion |
| 290 | Sweater | Zara | Men's Fashion |
| 413 | Jeans | Zara | Women's Fashion |
| 534 | Dress | Adidas | Kids' Fashion |
| 579 | Shoes | Gucci | Women's Fashion |
| 939 | Jeans | H&M | Men's Fashion |
| 970 | Sweater | H&M | Kids' Fashion |
| 989 | T-shirt | Adidas | Men's Fashion |
| 992 | T-shirt | Gucci | Women's Fashion |

---

# 📈 Model Evaluation

Dua metode rekomendasi dievaluasi menggunakan metrik yang berbeda sesuai karakteristik masing-masing pendekatan.

## 1. Content-Based Filtering

Evaluasi Content-Based Filtering menggunakan metrik klasifikasi.

| Metric | Score |
|----------|-------|
| Precision | **1.0000** |
| Recall | **1.0000** |
| F1-Score | **1.0000** |
| Accuracy | **1.0000** |

### Insight

- Seluruh produk yang direkomendasikan dianggap relevan terhadap produk acuan.
- Nilai evaluasi mencapai **100%**, menunjukkan bahwa sistem berhasil mengembalikan seluruh produk yang termasuk dalam daftar produk paling mirip.
- Perlu diperhatikan bahwa evaluasi ini menggunakan **ground truth berbasis data yang sama (dummy evaluation)** sehingga hasilnya bersifat ilustratif dan bukan evaluasi terhadap data baru.

---

## 2. Collaborative Filtering

Evaluasi Collaborative Filtering dilakukan menggunakan metrik error prediksi rating.

| Metric | Score |
|----------|-------|
| RMSE | **1.1268** |
| MAE | **0.9818** |

### Insight

- Model memiliki rata-rata kesalahan prediksi sekitar **±1 poin rating**.
- Nilai **MAE lebih kecil daripada RMSE**, yang menunjukkan bahwa sebagian besar kesalahan prediksi tidak terlalu ekstrem.
- Performa model masih dapat ditingkatkan melalui hyperparameter tuning, penggunaan algoritma lain, maupun penambahan data interaksi pengguna.

---

# 📊 Evaluation Summary

| Model | Result | Insight |
|--------|--------|---------|
| Content-Based Filtering | Precision, Recall, F1, Accuracy = **1.00** | Memberikan rekomendasi yang sangat relevan berdasarkan kemiripan atribut produk. |
| Collaborative Filtering | RMSE = **1.13**, MAE = **0.98** | Mampu mempelajari preferensi pengguna dengan performa yang cukup baik dan masih dapat ditingkatkan. |

---

# 💡 Recommendation Examples

## Content-Based Filtering

Input Product

```
Product ID : 1
```

Output

```
Dress - Adidas
Dress - Adidas
Jeans - Adidas
Dress - H&M
Dress - H&M
Dress - H&M
Sweater - Adidas
Dress - Adidas
Dress - H&M
Dress - H&M
```

---

## Collaborative Filtering

Input User

```
User ID : 19
```

Output

```
T-shirt - Zara
Dress - Gucci
Sweater - Zara
Jeans - Zara
Dress - Adidas
Shoes - Gucci
Jeans - H&M
Sweater - H&M
T-shirt - Adidas
T-shirt - Gucci
```

---

# 🚀 Installation

Clone repository.

```bash
git clone https://github.com/apriliaaamelani/fashion-product-recommendation-system.git
```

Masuk ke folder project.

```bash
cd fashion-product-recommendation-system
```

Install seluruh dependency.

```bash
pip install -r requirements.txt
```

---

# ▶️ Run Project

Menjalankan Notebook.

```bash
jupyter notebook
```

atau

```bash
jupyter lab
```

Kemudian buka file

```
recommendation_system.ipynb
```

Apabila ingin menjalankan script Python secara langsung.

```bash
python recommendation_system.py
```

---

# 📚 References

- Fashion Products Dataset

  https://www.kaggle.com/datasets/bhanupratapbiswas/fashion-products

- Ricci, F., Rokach, L., & Shapira, B. (2015). *Recommender Systems Handbook.*

- Bobadilla, J., Ortega, F., Hernando, A., & Gutiérrez, A. (2013). *Recommender Systems Survey.*

- Zhao, X., Zhang, Y., & Xu, K. (2020). *A Hybrid Recommendation System for Fashion E-commerce.*

---

# 🚀 Future Improvements

Beberapa pengembangan yang dapat dilakukan pada proyek ini antara lain:

- Hyperparameter tuning pada model SVD.
- Mengimplementasikan algoritma KNN-Based Recommendation.
- Menggunakan Neural Collaborative Filtering.
- Mengembangkan Hybrid Recommendation System.
- Menambahkan antarmuka berbasis web menggunakan Streamlit atau Flask.
- Membangun REST API untuk layanan rekomendasi.
- Deployment menggunakan Docker dan cloud platform.

---

# 🛠 Skills Demonstrated

Project ini menunjukkan kemampuan pada bidang berikut.

- Recommendation System
- Machine Learning
- Feature Engineering
- Natural Language Processing
- TF-IDF Vectorization
- Cosine Similarity
- Collaborative Filtering
- Singular Value Decomposition (SVD)
- Model Evaluation
- Data Visualization
- Data Analysis
- Python Programming

---

# 👩‍💻 Author

**Aprilia Melani**

Machine Learning Enthusiast | Data Analyst | AI Developer

LinkedIn

> https://www.linkedin.com/in/aprilia-melani-9698a8324/

---

# ⭐ Acknowledgements

Project ini dikembangkan sebagai implementasi Machine Learning pada bidang **Recommendation System** menggunakan dataset Fashion Products dari Kaggle.

Repository ini bertujuan sebagai portofolio yang menunjukkan kemampuan dalam membangun sistem rekomendasi menggunakan pendekatan **Content-Based Filtering** dan **Collaborative Filtering** dengan Python.

Apabila repository ini bermanfaat, jangan ragu untuk memberikan ⭐ pada repository ini.
