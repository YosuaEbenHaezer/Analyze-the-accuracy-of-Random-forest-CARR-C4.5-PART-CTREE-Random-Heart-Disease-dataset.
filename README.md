💓 Prediksi Penyakit Jantung Menggunakan Berbagai Metode Klasifikasi di R
Proyek ini bertujuan untuk memprediksi kemungkinan penyakit jantung berdasarkan dataset yang diberikan menggunakan beberapa metode klasifikasi populer di R. Algoritma yang digunakan meliputi CART (rpart), CTREE (party), Bagging (ipred), Boosting (C5.0), Naive Bayes, KNN, dan Random Forest.

📁 Dataset
File yang digunakan dalam proyek ini:

heart_disease_dataset.csv — sebagai data latih

heart_disease_dataset-testing.csv — sebagai data uji

Pastikan file ini berada dalam direktori kerja (working directory) R kamu.

📦 Library yang Digunakan
Berikut daftar lengkap library R yang digunakan dalam analisis ini:

r
Salin kode
# Decision Tree (CART dan CTREE)
library(rpart)
library(rpart.plot)
library(rattle)
library(party)

# Bagging (Bootstrap Aggregating)
library(ipred)

# Boosting (C5.0)
library(C50)

# Naive Bayes
library(klaR)
library(e1071)

# K-Nearest Neighbors
library(class)
library(caret)

# Random Forest
library(randomForest)

# WEKA (jika diperlukan)
library(RWeka)
library(rJava)
🔁 Beberapa library mungkin diulang karena dibutuhkan oleh lebih dari satu algoritma.

🚀 Cara Menjalankan Proyek
Buka file RMarkdown atau R Script:
File utama adalah UjianSisipan_215314148_rangkuman.Rmd.

Pastikan semua package telah terinstal:
Jika belum, jalankan:

r
Salin kode
install.packages("nama_package")
Jalankan kode secara berurutan:

Mulai dari memuat data.

Lakukan preprocessing seperti konversi tipe data, penanganan missing value, dll.

Latih model dan lakukan prediksi.

Evaluasi akurasi dan tampilkan hasil visualisasi pohon atau confusion matrix.

Untuk menjalankan .Rmd bisa klik Knit di RStudio atau jalankan setiap chunk secara manual.

📊 Output yang Dihasilkan
Visualisasi model decision tree (CART & CTREE)

Confusion matrix dan nilai akurasi untuk masing-masing model

Perbandingan performa antar metode klasifikasi

Prediksi







Anda bilang:
buat dalam format readme sehingga tinggal disalin


ChatGPT bilang:
Berikut README dalam format lengkap dan siap disalin ke file README.md:

markdown
Salin kode
# 💓 Prediksi Penyakit Jantung Menggunakan Berbagai Metode Klasifikasi di R

Proyek ini bertujuan untuk memprediksi kemungkinan penyakit jantung berdasarkan dataset yang diberikan menggunakan beberapa metode klasifikasi populer di R. Algoritma yang digunakan meliputi **CART (rpart)**, **CTREE (party)**, **Bagging (ipred)**, **Boosting (C5.0)**, **Naive Bayes**, **KNN**, dan **Random Forest**.

## 📁 Dataset

File yang digunakan dalam proyek ini:

- `heart_disease_dataset.csv` — sebagai **data latih**
- `heart_disease_dataset-testing.csv` — sebagai **data uji**

Pastikan kedua file berada dalam direktori kerja (working directory) R kamu.

## 📦 Library yang Digunakan

Berikut daftar lengkap library R yang digunakan dalam analisis ini:

```r
# CART dan CTREE
library(rpart)
library(rpart.plot)
library(rattle)
library(party)

# Bagging
library(ipred)

# Boosting
library(C50)

# Naive Bayes
library(klaR)
library(e1071)

# K-Nearest Neighbors (KNN)
library(class)
library(caret)

# Random Forest
library(randomForest)

# WEKA (jika diperlukan)
library(RWeka)
library(rJava)
🔁 Beberapa library mungkin diulang karena dibutuhkan oleh lebih dari satu algoritma.

🚀 Cara Menjalankan
Buka file utama
File utama adalah: UjianSisipan_215314148_rangkuman.Rmd

Pastikan semua package telah terinstal
Jika belum, jalankan:

r
Salin kode
install.packages("nama_package")
Jalankan kode secara berurutan

Mulai dari pemanggilan library dan load data.

Lakukan preprocessing (konversi faktor, normalisasi, pengecekan missing value).

Latih model dan prediksi terhadap data uji.

Evaluasi hasil dengan confusion matrix dan akurasi.

Visualisasikan model decision tree dengan rpart.plot atau fancyRpartPlot.

Untuk menjalankan file .Rmd

Gunakan tombol Knit di RStudio untuk menghasilkan laporan HTML/PDF.

Atau jalankan per blok kode (chunk) secara manual.

📊 Output yang Dihasilkan
Visualisasi model decision tree (CART dan CTREE)

Confusion matrix untuk masing-masing model

Akurasi prediksi data uji

Perbandingan performa antar model klasifikasi

📝 Catatan
Gunakan set.seed() untuk hasil yang reprodusibel.

Perhatikan distribusi target dan balancing data jika perlu.

Data testing (heart_disease_dataset-testing.csv) hanya digunakan untuk evaluasi akhir, bukan pelatihan model.
