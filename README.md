# Analisis_Sentimen

# 🎮 Analisis Sentimen Komentar Game AOV di Play Store

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qfv9gfDdyLF9sQ0R5RByfScE2zoa5Hvy)

Proyek ini bertujuan untuk **menganalisis sentimen pengguna terhadap game di Google Play Store**, dengan mengelompokkan komentar menjadi dua kategori utama:
- 🟢 **Positif**
- 🔴 **Negatif**

Notebook ini dikembangkan dan dijalankan sepenuhnya di **Google Colab**, dengan bahasa pemrograman **Python** serta dukungan berbagai library analisis data dan pembelajaran mesin.

---

## 🧠 Deskripsi Proyek

Analisis sentimen ini bertujuan untuk memahami **persepsi pemain terhadap game tertentu di Play Store**.  
Dengan klasifikasi komentar pengguna, pengembang dapat mengetahui seberapa baik penerimaan publik terhadap game, serta menemukan area yang perlu ditingkatkan.

### 🔍 Alur Analisis:
1. **Pengumpulan Data**  
   Mengambil komentar dari Play Store (melalui scraping atau dataset yang sudah tersedia).

2. **Prapemrosesan (Preprocessing)**  
   - Case folding  
   - Stopword removal  
   - Tokenisasi  
   - Stemming menggunakan *Sastrawi*

3. **Klasifikasi Sentimen**  
   Menggunakan model seperti:
   - Naive Bayes  
   - Logistic Regression  
   - Support Vector Machine (SVM)

4. **Evaluasi Model**  
   Mengukur akurasi, precision, recall, dan f1-score.

5. **Visualisasi Hasil**  
   Menampilkan sebaran sentimen dan *wordcloud* dari kata yang paling sering muncul.

---

## ⚙️ Teknologi dan Library yang Digunakan

| Kategori | Library |
|-----------|----------|
| Analisis Data | `pandas`, `numpy` |
| Pemrosesan Teks | `nltk`, `sastrawi` |
| Ekstraksi Fitur & Model | `scikit-learn` |
| Visualisasi | `matplotlib`, `seaborn`, `wordcloud` |
| Platform | `Google Colab` |

---

## 📂 Struktur Notebook

.
├── dataset/ # Dataset komentar pengguna Play Store
├── preprocessing/ # Tahap pembersihan dan normalisasi teks
├── models/ # Model Machine Learning yang digunakan
├── results/ # Hasil evaluasi dan visualisasi
└── README.md # Dokumentasi proyek

## 🚀 Cara Menjalankan

1. Klik tombol **“Open in Colab”** di atas, atau buka secara manual:  
   👉 [https://colab.research.google.com/drive/1qfv9gfDdyLF9sQ0R5RByfScE2zoa5Hvy](https://colab.research.google.com/drive/1qfv9gfDdyLF9sQ0R5RByfScE2zoa5Hvy)

2. Jalankan semua sel kode secara berurutan (Ctrl + F9).

3. Upload dataset komentar (`.csv` atau `.xlsx`) ke Colab:
   ```python
   from google.colab import files
   uploaded = files.upload()
Setelah dijalankan, hasil akan menampilkan:

Grafik akurasi model

Wordcloud

Confusion Matrix

Persentase komentar positif dan negatif

📊 Contoh Output
Visualisasi	Deskripsi
📈 Grafik Akurasi	Performa model terhadap data uji
☁️ Wordcloud	Kata yang paling sering muncul pada tiap sentimen
🔵 Confusion Matrix	Perbandingan prediksi benar dan salah
📊 Distribusi Sentimen	Persentase komentar positif vs negatif

📄 Lisensi
Proyek ini dilisensikan di bawah MIT License — bebas digunakan, dimodifikasi, dan disebarluaskan dengan tetap mencantumkan kredit kepada pembuat aslinya.

✨ Author
  Shinee33
💻 Dibuat dengan ❤️ menggunakan Google Colab
📊 Fokus: Analisis Sentimen Ulasan Game AOV Play Store
