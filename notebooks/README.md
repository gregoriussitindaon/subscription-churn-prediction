# Telco Customer Churn Prediction

## 1. Latar Belakang Bisnis

Churn pelanggan merupakan salah satu sumber kebocoran pendapatan paling signifikan bagi perusahaan berbasis langganan (subscription) seperti telekomunikasi, SaaS, dan layanan digital. Mengidentifikasi pelanggan dengan risiko churn tinggi sebelum mereka benar-benar berhenti adalah langkah kunci untuk menekan biaya akuisisi ulang dan menjaga stabilitas pendapatan.

Proyek ini mensimulasikan kasus nyata menggunakan dataset Telco Customer Churn dan menunjukkan bagaimana analisis berbasis Python dapat:
- memetakan faktor pendorong churn,
- membangun model prediktif,
- menghasilkan rekomendasi retensi yang operasional.

## 2. Tujuan

- Membangun model prediksi churn yang interpretable dan usable.
- Mengidentifikasi faktor utama penyebab churn.
- Menyusun rekomendasi strategi retensi pelanggan berisiko tinggi.

## 3. Data

- Sumber: Telco Customer Churn dataset (IBM sample, via Kaggle).
- Target: `Churn` (Yes/No) → dikonversi menjadi label biner.
- Fitur utama:
  - lama berlangganan (tenure),
  - jenis kontrak,
  - metode pembayaran,
  - layanan yang digunakan,
  - biaya bulanan & total.

Dataset asli tidak disertakan dalam repository ini. Pengguna dapat mengunduh dari Kaggle dan menempatkannya di `data/raw/`.

## 4. Metodologi

1. Data cleaning & preprocessing.
2. Exploratory Data Analysis (EDA) untuk memahami profil pelanggan churn vs non-churn.
3. Encoding fitur kategorikal & scaling fitur numerik.
4. Pembangunan model:
   - Logistic Regression (baseline, interpretable),
   - Random Forest (non-linear, feature importance).
5. Evaluasi menggunakan:
   - Confusion matrix, precision, recall, F1-score,
   - ROC-AUC.
6. Interpretasi feature importance untuk faktor penyebab churn.
7. Rekomendasi bisnis berdasarkan temuan model.

## 5. Notebook

Analisis lengkap terdapat pada:

`notebooks/01_churn_eda_model.ipynb`

## 6. Teknologi

- Python: pandas, numpy, scikit-learn, matplotlib, seaborn
- Google Colab / Jupyter Notebook
- GitHub untuk dokumentasi & version control

## 7. Output Utama

- Model klasifikasi churn dengan metrik evaluasi yang transparan.
- Daftar faktor risiko churn prioritas.
- Rekomendasi strategi retensi yang dapat langsung dikomunikasikan ke tim bisnis.
