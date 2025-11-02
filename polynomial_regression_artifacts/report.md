# Polynomial Regression Project - Report

## 1. Executive Summary
- Dataset: 300 sampel properti
- Best Polynomial Degree: 2
- Best CV R² (Linear Model): 0.8106
- Best Regularization (Degree=2): Ridge alpha=10, R²=0.7986

## 2. Insights dari EDA
- Fitur Luas_Bangunan_m2 & Luas_Tanah_m2 memiliki korelasi positif terhadap harga.
- Jarak_ke_Pusat_km berkorelasi negatif terhadap harga.
- Outlier terlihat pada Luas_Tanah_m2 dan Harga_Juta.

## 3. Perbandingan Performa Model
|   degree | model   |   train_r2 |     test_r2 |
|---------:|:--------|-----------:|------------:|
|        1 | Linear  |   0.814298 |   0.820541  |
|        2 | Linear  |   0.854844 |   0.797498  |
|        3 | Linear  |   0.873502 |   0.778438  |
|        4 | Linear  |   0.92185  |   0.0939298 |
|        5 | Linear  |   1        | -17.3293    |

## 4. Rekomendasi
- Polynomial Degree terbaik: 2
- Regularization terbaik: Ridge (alpha=10)

## 5. Limitasi Model
- Fitur terbatas, belum mencakup lokasi mikro & kondisi bangunan.
- Sensitif terhadap outlier besar.
- CI prediksi berbasis residual sederhana.

## 6. Saran Improvement
- Tambahkan fitur kualitatif (lingkungan, fasilitas).
- Gunakan model tree-based (RandomForest/XGBoost).
- Evaluasi dengan cross-validation lebih kompleks.
