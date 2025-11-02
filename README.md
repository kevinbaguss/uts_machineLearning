# 🏡 Polynomial Regression Project

Proyek ini bertujuan untuk membuat model **Polynomial Regression** yang dapat memprediksi harga properti berdasarkan fitur-fitur seperti luas tanah, luas bangunan, jumlah kamar, umur bangunan, dan jarak ke pusat kota.

Model dilatih menggunakan **dataset sintetis** yang dihasilkan secara otomatis dan mencakup analisis data eksploratif (EDA), pelatihan model dengan beberapa derajat polinomial, validasi silang, serta penerapan regularisasi (Ridge & Lasso).

---

## 📦 1. Cara Install Dependencies

### a. Clone Repository
Pastikan sudah memiliki Python 3.8+ dan `pip`. :
```bash
pip install -r requirements.txt
```

## 2. cara menjalankan script: 
run satu per satu script dari paling atas sampai bawah.

setelah itu Script ini akan:
Membuat dataset sintetik properti (jika belum ada).
Menjalankan EDA (histogram, scatter plot, heatmap, boxplot).
Melatih model Polynomial Regression dengan berbagai derajat.
Melakukan validasi silang (cross-validation).
Menguji regularisasi Ridge dan Lasso.
Menyimpan model terbaik dan laporan hasil di folder:

```bash
./polynomial_regression_artifacts/
```
## 3 Struktur folder
```bash
uts_machineLearning/
│
│
├── polynomial_regression_artifacts/   # Folder keluaran otomatis berisi model dan laporan
│   ├── synthetic_property_data.csv     # Dataset sintetik
│   ├── best_model.pkl                  # Model polynomial regression terbaik (disimpan dengan joblib)
│   ├── best_poly.pkl                   # PolynomialFeatures object untuk transformasi input
│   ├── scaler.pkl                      # StandardScaler untuk normalisasi data
│   └── report.md                       # Laporan hasil eksperimen
│
├── requirements.txt                   # Daftar library Python yang dibutuhkan
│
└── README.md                          # Dokumentasi proyek (file ini)
```


