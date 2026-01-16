🚗 Prediksi Harga Mobil Menggunakan Machine Learning
📌 Deskripsi Proyek

Proyek ini bertujuan untuk memprediksi harga mobil berdasarkan beberapa fitur penting menggunakan metode Machine Learning (Regression).
Model dibangun melalui tahapan lengkap mulai dari data preprocessing, EDA, feature engineering, hingga evaluasi model.

Proyek ini cocok sebagai latihan end-to-end machine learning workflow untuk pemula.

📂 Dataset

Dataset yang digunakan adalah data_car.csv, yang berisi informasi terkait spesifikasi mobil seperti:

Brand / Model

Tahun

Transmisi

Fuel type

Mileage

Engine

Power

Seats

Harga mobil (target)

⚙️ Library yang Digunakan
pandas
numpy
matplotlib
seaborn
scikit-learn

🔄 Alur Pengerjaan Proyek
1️⃣ Import Library & Load Data

Mengimpor library yang dibutuhkan

Membaca dataset menggunakan pandas

2️⃣ Data Cleaning & Preprocessing

Beberapa tahapan preprocessing yang dilakukan:

Menghapus kolom yang tidak relevan

Menghapus data duplikat

Menangani missing values

Memisahkan fitur numerik dan kategorikal

Encoding fitur kategorikal

Scaling fitur numerik

Semua preprocessing digabung menggunakan Pipeline & ColumnTransformer untuk menghindari data leakage.

3️⃣ Exploratory Data Analysis (EDA)

Melihat distribusi data

Visualisasi hubungan fitur dengan harga mobil

Scatter plot antara nilai aktual dan prediksi

4️⃣ Train-Test Split

Data dibagi menjadi:

Training set

Testing set

Menggunakan:

train_test_split()

5️⃣ Model Machine Learning

Model yang digunakan:

Linear Regression

Model diimplementasikan dalam Pipeline agar preprocessing dan training berjalan otomatis.

6️⃣ Evaluasi Model

Metrik evaluasi yang digunakan:

R² Score

Mean Absolute Error (MAE)

Evaluasi dilakukan pada:

Data training

Data testing

7️⃣ Visualisasi Hasil Prediksi

Scatter plot Actual vs Predicted

Garis diagonal untuk melihat seberapa dekat prediksi dengan nilai aktual

📊 Hasil & Insight

Model mampu mempelajari pola harga mobil dengan cukup baik

Selisih prediksi dapat dilihat melalui visualisasi

Cocok sebagai baseline model sebelum mencoba algoritma lain seperti:

Random Forest

XGBoost

Gradient Boosting

🚀 Pengembangan Selanjutnya

Beberapa improvement yang bisa dilakukan:

Menggunakan model non-linear

Hyperparameter tuning

Feature selection

Deploy model ke web app (Streamlit)

🧠 Kesimpulan

Proyek ini menunjukkan bagaimana membangun model regresi dari awal hingga evaluasi dengan workflow yang rapi dan aman dari data leakage menggunakan Pipeline.
