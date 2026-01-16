# Analisis & Prediksi Harga Mobil (Car Price Prediction) 🚗💰

Proyek ini adalah sebuah **Jupyter Notebook** yang bertujuan untuk melakukan analisis data eksploratif (*Exploratory Data Analysis*) dan pembersihan data (*Data Cleaning*) pada dataset harga mobil. Tujuannya adalah untuk memahami faktor-faktor yang mempengaruhi harga jual mobil (MSRP) dan mempersiapkan data yang bersih untuk pemodelan lebih lanjut.

## 📋 Daftar Isi
- [Gambaran Proyek](#gambaran-proyek)
- [Dataset](#dataset)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Alur Kerja (Workflow)](#alur-kerja-workflow)
- [Fitur Data](#fitur-data)
- [Cara Menjalankan](#cara-menjalankan)

## 📖 Gambaran Proyek
Dalam notebook ini, kita memproses data mentah spesifikasi mobil untuk mendapatkan *insight* yang lebih jelas. Langkah-langkah utama meliputi penghapusan data yang tidak relevan, standarisasi nama kolom, penanganan data ganda (*duplicates*), serta deteksi *outlier* menggunakan visualisasi.

## 💾 Dataset
Proyek ini menggunakan dataset **`data_car.csv`**.
> **Catatan:** Pastikan file `data_car.csv` berada dalam satu folder yang sama dengan file notebook saat dijalankan.

## 🛠 Teknologi yang Digunakan
Analisis ini dibuat menggunakan bahasa pemrograman **Python** dengan library berikut:
* **Pandas**: Untuk manipulasi dan analisis struktur data.
* **NumPy**: Untuk operasi numerik.
* **Matplotlib** & **Seaborn**: Untuk visualisasi data (membuat grafik dan plot).

## 🚀 Alur Kerja (Workflow)
Berikut adalah tahapan analisis yang dilakukan dalam file `Memprediksi_harga_Mobil.ipynb`:

1.  **Import Library & Load Data**: Memuat library Python yang dibutuhkan dan membaca dataset.
2.  **Data Cleaning (Pembersihan Data)**:
    * **Menghapus Kolom**: Mengeliminasi kolom yang dianggap kurang relevan untuk analisis harga, seperti *Engine Fuel Type, Market Category, Number of Doors, Popularity, Vehicle Size,* dan *Vehicle Style*.
    * **Rename Kolom**: Mengubah nama kolom agar lebih singkat dan mudah dipahami (contoh: `Engine HP` ➔ `HP`, `MSRP` ➔ `Price`).
    * **Menghapus Duplikat**: Mendeteksi dan menghapus baris data yang identik (terdapat sekitar 989 data duplikat yang dibersihkan).
    * **Handling Missing Values**: Menghapus baris yang memiliki nilai kosong (null) untuk menjaga kualitas data.
3.  **Exploratory Data Analysis (EDA)**:
    * Mendeteksi **Outlier** (pencilan data) menggunakan visualisasi *Boxplot* pada fitur-fitur numerik utama:
        * `Year` (Tahun pembuatan)
        * `HP` (Tenaga mesin)
        * `Cylinders` (Jumlah silinder)
        * `MPG-H` (Konsumsi bahan bakar di jalan tol)

## 📊 Fitur Data
Setelah proses pembersihan, berikut adalah fitur-fitur utama yang digunakan:
* **Make**: Merek mobil (misal: BMW, Audi).
* **Model**: Model spesifik dari mobil.
* **Year**: Tahun pembuatan mobil.
* **HP**: Tenaga mesin (*Horsepower*).
* **Cylinders**: Jumlah silinder pada mesin.
* **Transmission**: Tipe transmisi (Manual/Automatic).
* **Drive Mode**: Sistem penggerak roda (FWD, RWD, AWD).
* **MPG-H**: Efisiensi bahan bakar di jalan tol (*Highway MPG*).
* **MPG-C**: Efisiensi bahan bakar dalam kota (*City MPG*).
* **Price**: Harga jual mobil (*Manufacturer's Suggested Retail Price*).

## 💻 Cara Menjalankan
1.  Pastikan kamu sudah menginstal Python dan Jupyter Notebook.
2.  Install library yang dibutuhkan dengan menjalankan perintah berikut di terminal:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Clone atau download repositori ini.
4.  Buka terminal/command prompt di direktori folder proyek.
5.  Jalankan Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
6.  Buka file `Memprediksi_harga_Mobil.ipynb` dan jalankan setiap sel (*cell*) kodenya.

---
*Dibuat untuk tujuan pembelajaran Data Science dan Analisis Data.*
