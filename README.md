# Laporan Proyek Machine Learning - Dimas NurHamzah
## Project Overview
Latar Belakang dari masalah ini adalah, keinginan membuat sistem yang dapat merekomendasikan game pada sistem aplikasi 
## Business Understanding
* Problem statement:
  * Bagaimana membuat sistem rekomendasi yang dipersonalisasi dengan teknik content-based filtering?
  * Dengan data genre game yang ada, bagaimana sistem dapat merekomendasikan game lain yang mungkin disukai dan belum pernah dikunjungi oleh pengguna?
* Goals
  * Menghasilkan sejumlah rekomendasi restoran yang dipersonalisasi untuk pengguna dengan teknik content-based filtering
  * Menghasilkan sejumlah rekomendasi restoran yang sesuai dengan preferensi pengguna dan belum pernah dikunjungi sebelumnya dengan teknik collaborative filtering
## Data Understanding 
* Pada Proyek ini menggunakan dataset "https://www.kaggle.com/datasets/gregorut/videogamesales" dataset ini memiliki mememiliki 16598 rows × 11 columns, tetapi saya hanya menggunakan 3 kolom yaitu : 
   * Rank merupakan id pada dataset
   * Name merupakan nama game pada dataset
   * Genre merupakan kategori game pada dataset
## Data Preparation
* Pada tahap ini, saya melakukan cek missing value,lalu membersihkan missing value dengan fungsi dropna
* Dan menghapus data yang duplikat dengan fungsi drop_duplicates()
## Modeling 
* Penyelesain masalah dengan Content based Filtering, tahapan melakukan model yaitu: 
  * Dengan TF-IDF Vectorizer, untuk membangun sistem sederhana berdasarkan genre dari game
  * Tahapan: import TfidfVectorizer
  * lalu melakukan perhitungan pada data genre
  * Selanjutnya melakukan fit dan mentransformasi data kedalam bentuk matriks 
  * Lalu menggunakan fungsi todense untuk menghasilkan vektor tf-idf, yang akan digunakan untuk melihat korelasi antara genre dengan nama
## Evaluasi
 * 
