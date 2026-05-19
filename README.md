# Analisis Sentimen Ulasan Aplikasi Portal Pulsa pada Google Play Store Menggunakan Metode Machine Learning

Proyek ini bertujuan untuk menganalisis sentimen ulasan pengguna aplikasi Portal Pulsa di Google Play Store dengan membandingkan performa 4 algoritma Machine Learning.

## 📊 Ringkasan Dataset & Preprocessing
* **Sumber Data:** Data ulasan (scraping) dari Google Play Store.
* **Total Data Awal:** 12.000 ulasan.
* **Total Data Setelah Preprocessing:** 11.604 ulasan (setelah pembersihan data kosong/duplikat).
* **Tahapan Preprocessing:** 1. Case Folding
  2. Cleansing (Pembersihan simbol, angka, dan emoji)
  3. Tokenizing
  4. Normalisasi Kata (Mengubah kata alay/singkatan)
  5. Stopword Removal (Menggunakan Sastrawi)
  6. Stemming (Menggunakan Sastrawi)
* **Pelabelan Sentimen:** Menggunakan kamus leksikon (*Lexicon-based*) ke dalam 2 kelas, yaitu **Sentimen Positif** dan **Sentimen Negatif**.
* **Ekstraksi Fitur:** TF-IDF Vectorizer.

## 🛠️ Tech Stack & Library
* **Bahasa Pemrograman:** Python
* **Environment:** Google Colab
* **Library Utama:** `pandas`, `numpy`, `scikit-learn`, `nltk`, `Sastrawi`.

## 📈 Hasil Perbandingan Akurasi Model
Pengujian dilakukan dengan membandingkan 4 algoritma menggunakan pembagian data training dan data testing. Berikut adalah hasil akurasi terbaik dari masing-masing algoritma:

1. **Support Vector Machine (SVM):** **93.28%** (Performa Tertinggi 🏆)
2. **Naïve Bayes (MultinomialNB):** **89.57%**
3. **Decision Tree:** **89.31%**
4. **K-Nearest Neighbors (KNN):** **84.36%**

## 💡 Kesimpulan
Algoritma **Support Vector Machine (SVM)** memberikan hasil performa terbaik dalam mengklasifikasikan sentimen ulasan aplikasi Portal Pulsa dengan tingkat akurasi mencapai **93.28%**, diikuti oleh Naïve Bayes dan Decision Tree, sementara KNN memiliki akurasi terendah pada dataset ini.
