# 🚗 Prediksi Harga Mobil Menggunakan Machine Learning

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk **memprediksi harga mobil** berdasarkan berbagai fitur menggunakan metode **Machine Learning (Regression)**.  
Model dibangun melalui tahapan lengkap mulai dari **data preprocessing**, **Exploratory Data Analysis (EDA)**, hingga **evaluasi model**.

Proyek ini dibuat sebagai latihan **end-to-end machine learning workflow**.

---

## 📂 Dataset
Dataset yang digunakan adalah `data_car.csv`, yang berisi informasi spesifikasi mobil, seperti:
- Brand / Model
- Tahun
- Transmisi
- Jenis bahan bakar
- Mileage
- Engine
- Power
- Seats
- Harga mobil (target)

---

## ⚙️ Library yang Digunakan
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

---

## 🔄 Alur Pengerjaan Proyek

### 1. Import Library & Load Data
Mengimpor library yang dibutuhkan dan membaca dataset menggunakan pandas.

### 2. Data Cleaning & Preprocessing
Tahapan preprocessing yang dilakukan:
- Menghapus kolom yang tidak relevan
- Menghapus data duplikat
- Menangani missing values
- Encoding fitur kategorikal
- Scaling fitur numerik  

Seluruh preprocessing dilakukan menggunakan **Pipeline** dan **ColumnTransformer** untuk menghindari data leakage.

### 3. Exploratory Data Analysis (EDA)
- Analisis distribusi data
- Visualisasi hubungan fitur terhadap harga mobil

### 4. Train-Test Split
Data dibagi menjadi data training dan testing menggunakan `train_test_split`.

### 5. Model Machine Learning
Model yang digunakan:
- **Linear Regression**

Model diimplementasikan menggunakan pipeline agar preprocessing dan training berjalan otomatis.

### 6. Evaluasi Model
Model dievaluasi menggunakan metrik:
- R² Score
- Mean Absolute Error (MAE)

Evaluasi dilakukan pada data training dan testing.

### 7. Visualisasi Hasil
- Visualisasi perbandingan nilai aktual dan nilai prediksi menggunakan scatter plot.

---

## 📊 Hasil
Model mampu mempelajari pola harga mobil dengan cukup baik dan dapat dijadikan **baseline model** untuk pengembangan lebih lanjut.

---

## 🚀 Pengembangan Selanjutnya
- Menggunakan model yang lebih kompleks (Random Forest, XGBoost)
- Hyperparameter tuning
- Feature selection
- Deployment ke web app (Streamlit)

---

## 🧠 Kesimpulan
Proyek ini menunjukkan proses lengkap pembuatan model regresi mulai dari preprocessing hingga evaluasi dengan workflow yang rapi dan aman dari data leakage.

---

