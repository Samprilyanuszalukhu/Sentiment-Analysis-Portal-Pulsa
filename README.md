# Analisis Sentimen Ulasan Aplikasi Portal Pulsa pada Google Play Store Menggunakan Metode Machine Learning

# penelitian untuk SKRIPSI

Proyek ini bertujuan untuk menganalisis sentimen ulasan pengguna aplikasi Portal Pulsa di Google Play Store dengan membandingkan performa 4 algoritma Machine Learning.

## 📊 Ringkasan Dataset & Preprocessing
* **Sumber Data:** Data ulasan (scraping) dari Google Play Store.
* **Total Data Awal:** 4.302 ulasan.
* **Total Data Setelah Preprocessing:**4.302 ulasan (setelah pembersihan data kosong/duplikat).
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

# analisis-sentimen-portal-pulsa  
<img width="762" height="349" alt="pertama" src="https://github.com/user-attachments/assets/837a9a02-50cd-418f-994b-6964c19807e5" />
#Pelabelan negatif (Labeling)
<img width="669" height="525" alt="labeling" src="https://github.com/user-attachments/assets/88ce5968-8e77-400c-8a2c-b241ae7c335e" />

# pelabelan positif (labeling)
<img width="692" height="525" alt="label positif" src="https://github.com/user-attachments/assets/a704a84f-b268-4ca7-8058-5b67ff18c5e7" />

# Hasil grafik batang pelabelan
<img width="622" height="563" alt="grafik" src="https://github.com/user-attachments/assets/a0c94925-13b4-40da-bc62-a234240934fe" />

# Hasil Visual WordCloud
<img width="895" height="303" alt="Hasil Visual WordCloud" src="https://github.com/user-attachments/assets/9dc25f81-cac3-4caa-b310-41ed88eedc36" />

# Hasil Pembobotan (TD-IDF)
<img width="845" height="176" alt="Hasil Pembobotan" src="https://github.com/user-attachments/assets/d4a95925-dd1d-4f15-8205-cd9c772cb68c" />

# Grafik Batang Cross Validation
<img width="793" height="396" alt="Grafik Batang Cross Validation" src="https://github.com/user-attachments/assets/43a74a79-364c-4ddf-abcc-02e35e82b2fc" />

# Hasil Uji Anova dan Paired T-Test 
<img width="403" height="168" alt="Hasil Uji Anova dan Paired T-Test" src="https://github.com/user-attachments/assets/227541fa-d207-4613-b7c1-1d3b8ef966e0" />

# Confusion Matrix Linear Svm.
<img width="536" height="397" alt="Confusion Matrix Linear Svm" src="https://github.com/user-attachments/assets/2adb0566-6044-497f-9aa2-f0766c2c1ed7" />

# Fitur Positif dan Negatif pada Model Linear SVM
<img width="618" height="296" alt="Fitur Positif dan Negatif pada Model Linear SVM" src="https://github.com/user-attachments/assets/1c76fcbb-76cf-429f-9bee-30bec8692cc3" />

# Grafik Hasil Test Data
<img width="860" height="478" alt="Grafik Hasil Test Data" src="https://github.com/user-attachments/assets/dc1eda3c-4d31-4865-82a5-88d60737f914" />












4. **K-Nearest Neighbors (KNN):** **84.36%**

## 💡 Kesimpulan
Algoritma **Support Vector Machine (SVM)** memberikan hasil performa terbaik dalam mengklasifikasikan sentimen ulasan aplikasi Portal Pulsa dengan tingkat akurasi mencapai **93.28%**, diikuti oleh Naïve Bayes dan Decision Tree, sementara KNN memiliki akurasi terendah pada dataset ini.
