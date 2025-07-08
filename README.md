
# Analisis Sentimen Ulasan Aplikasi Viki

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna aplikasi Viki yang diambil dari Google Play Store. Analisis ini menggunakan tiga model machine learning dan deep learning yang berbeda, yaitu **Logistic Regression**, **Random Forest**, dan **Long Short-Term Memory (LSTM)** untuk membandingkan performa masing-masing model dalam mengklasifikasikan sentimen (positif, negatif, atau netral).

## latar Belakang

Viki adalah platform streaming video yang populer, terutama untuk drama dan film Asia. Ulasan pengguna di platform seperti Google Play Store merupakan sumber data yang kaya untuk memahami opini dan pengalaman pengguna. Dengan menganalisis sentimen dari ulasan ini, pengembang aplikasi dapat memperoleh wawasan berharga untuk meningkatkan kualitas aplikasi, memperbaiki bug, dan mengembangkan fitur baru.

## 🎯 Tujuan Proyek

  * Mengumpulkan dan membersihkan data ulasan aplikasi Viki.
  * Melakukan pra-pemrosesan teks pada ulasan untuk persiapan pemodelan.
  * Membangun dan melatih tiga model klasifikasi sentimen:
    1.  Logistic Regression
    2.  Random Forest
    3.  Long Short-Term Memory (LSTM)
  * Mengevaluasi dan membandingkan akurasi, presisi, recall, dan F1-score dari ketiga model.
  * Menentukan model terbaik untuk kasus studi analisis sentimen ulasan aplikasi Viki.

## Dataset

Dataset yang digunakan dalam proyek ini adalah kumpulan ulasan aplikasi Viki yang diambil dari Google Play Store. Ulasan ini mencakup teks ulasan dan rating bintang yang diberikan oleh pengguna, yang kemudian dilabeli menjadi sentimen positif, negatif, atau netral.

*(Anda bisa menambahkan detail lebih lanjut tentang dataset Anda di sini, misalnya jumlah data, periode pengambilan data, atau link ke dataset jika tersedia).*

## 🛠️ Teknologi dan Library

Proyek ini dibangun menggunakan bahasa pemrograman **Python** dengan beberapa library utama, di antaranya:

  * **Pandas:** Untuk manipulasi dan analisis data.
  * **NumPy:** Untuk komputasi numerik.
  * **Scikit-learn:** Untuk implementasi model Logistic Regression, Random Forest, dan metrik evaluasi.
  * **NLTK** atau **Sastrawi:** Untuk pra-pemrosesan teks Bahasa Indonesia (tokenization, stopword removal, stemming).
  * **TensorFlow & Keras:** Untuk membangun dan melatih model deep learning LSTM.
  * **Matplotlib & Seaborn:** Untuk visualisasi data dan hasil model.
  * **Jupyter Notebook:** Sebagai environment untuk pengembangan dan analisis interaktif.

## 📁 Struktur Repositori

```
.
├── data/
│   ├── raw_reviews.csv         # Data ulasan mentah
│   └── processed_reviews.csv   # Data ulasan setelah dibersihkan
├── notebooks/
│   ├── 01_data_exploration.ipynb   # Notebook untuk eksplorasi data
│   ├── 02_preprocessing.ipynb      # Notebook untuk pra-pemrosesan teks
│   ├── 03_modelling_logres_rf.ipynb# Notebook untuk model LogReg dan RF
│   └── 04_modelling_lstm.ipynb     # Notebook untuk model LSTM
├── src/
│   ├── data_loader.py            # Script untuk memuat data
│   ├── preprocessing.py          # Script untuk fungsi pra-pemrosesan
│   └── model_evaluation.py       # Script untuk fungsi evaluasi
├── models/
│   ├── logistic_regression.pkl   # Model Logistic Regression yang telah dilatih
│   ├── random_forest.pkl         # Model Random Forest yang telah dilatih
│   └── lstm_model.h5             # Model LSTM yang telah dilatih
├── requirements.txt                # Daftar library yang dibutuhkan
└── README.md                       # File ini
```

## ⚙️ Instalasi

Untuk menjalankan proyek ini di lingkungan lokal Anda, ikuti langkah-langkah berikut:

1.  **Clone repositori ini:**

    ```bash
    git clone https://github.com/URL_REPO_ANDA/nama-proyek.git
    cd nama-proyek
    ```

2.  **Buat dan aktifkan virtual environment (opsional namun direkomendasikan):**

    ```bash
    python -m venv venv
    # Windows
    venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```

3.  **Instal semua library yang dibutuhkan:**

    ```bash
    pip install -r requirements.txt
    ```

## 🚀 Cara Penggunaan

Anda dapat menjalankan analisis dengan membuka dan menjalankan file Jupyter Notebook secara berurutan di dalam direktori `notebooks/`:

1.  **Eksplorasi Data:** Buka `notebooks/01_data_exploration.ipynb` untuk melihat analisis data eksploratif.
2.  **Pra-pemrosesan:** Jalankan `notebooks/02_preprocessing.ipynb` untuk membersihkan dan mempersiapkan data.
3.  **Pemodelan:**
      * Untuk model Machine Learning, jalankan `notebooks/03_modelling_logres_rf.ipynb`.
      * Untuk model Deep Learning, jalankan `notebooks/04_modelling_lstm.ipynb`.

Hasil dari setiap model, termasuk metrik evaluasi dan confusion matrix, akan ditampilkan di dalam masing-masing notebook.

## 📈 Hasil

Proyek ini menghasilkan perbandingan performa antara model Logistic Regression, Random Forest, dan LSTM. Berdasarkan evaluasi, model **[Nama Model Terbaik, misal: LSTM]** menunjukkan performa terbaik dengan akurasi **[Contoh: 92%]** dan F1-score **[Contoh: 0.91]**. Hasil ini menunjukkan bahwa [jelaskan sedikit kesimpulan Anda, misalnya: "arsitektur deep learning lebih efektif dalam menangkap konteks dan nuansa dalam teks ulasan dibandingkan model machine learning klasik untuk dataset ini"].

## 🤝 Kontribusi

Kontribusi untuk pengembangan proyek ini sangat diterima. Jika Anda ingin berkontribusi, silakan lakukan *fork* pada repositori ini, buat *branch* baru untuk fitur atau perbaikan Anda, dan kirimkan *pull request*.
