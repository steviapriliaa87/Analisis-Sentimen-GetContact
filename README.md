# Analisis-Sentimen-GetContact

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna aplikasi **GetContact** yang diambil dari Google Play Store. Analisis ini dilakukan untuk mengidentifikasi sentimen (positif, netral, negatif) menggunakan berbagai pendekatan Machine Learning dan Deep Learning.

---

## 🧠 Metodologi

### 1. **Scraping Data**
- Mengambil data ulasan dari aplikasi GetContact menggunakan `google-play-scraper`.
- Hasil disimpan dalam file `ulasan_GetContact.csv`.

### 2. **Preprocessing**
- Menghapus duplikat dan stopwords.
- Case folding, tokenisasi, stemming, dan normalisasi kata.

### 3. **Pelabelan Sentimen**
- Menggunakan pendekatan **lexicon-based** untuk menentukan label sentimen secara otomatis.

### 4. **Training Model**
Melibatkan 3 pendekatan klasifikasi:
- **LSTM (Deep Learning)**  
- **SVM (Support Vector Machine)**  
- **Random Forest**

### 5. **Evaluasi**
- Menggunakan metrik akurasi, precision, recall, dan F1-score.
- Visualisasi Confusion Matrix.

### 6. **Inference**
- Notebook `Inference.ipynb` digunakan untuk prediksi sentimen terhadap input baru.

---

## 💼 Tools & Library

- Google Colab
- Python
- TensorFlow / Keras
- Scikit-learn
- NLTK & Sastrawi
- Pandas, NumPy
- Matplotlib, Seaborn

---

## 🚀 Cara Menjalankan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/Analisis-Sentimen-GetContact.git
   cd Analisis-Sentimen-GetContact

2. Install dependensi:
    ```bash
   pip install -r requirements.txt

---

## 📊 Hasil Akhir

Berikut adalah perbandingan akurasi dari masing-masing model klasifikasi sentimen:

| Model                       | Akurasi  |
|----------------------------|----------|
| LSTM + Embedding (80/20)   | **95.40%** |
| SVM + TF-IDF (80/20)       | **92.43%** |
| Random Forest + TF-IDF (80/20) | **88.55%** |

> Model LSTM memberikan performa terbaik dalam klasifikasi sentimen ulasan pengguna aplikasi GetContact.

---

## 📌 Catatan

- Model dan tokenizer telah diserialisasi dalam folder Models.

- Dataset ulasan bersumber langsung dari Google Play Store menggunakan scraping otomatis.




