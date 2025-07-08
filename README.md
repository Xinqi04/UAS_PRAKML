
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

## 🛠️ Teknologi dan Library

Proyek ini dibangun menggunakan bahasa pemrograman **Python** dengan beberapa library utama, di antaranya:

  * **Pandas:** Untuk manipulasi dan analisis data.
  * **NumPy:** Untuk komputasi numerik.
  * **Scikit-learn:** Untuk implementasi model Logistic Regression, Random Forest, dan metrik evaluasi.
  * **NLTK** atau **Sastrawi:** Untuk pra-pemrosesan teks Bahasa Indonesia (tokenization, stopword removal, stemming).
  * **TensorFlow & Keras:** Untuk membangun dan melatih model deep learning LSTM.
  * **Matplotlib & Seaborn:** Untuk visualisasi data dan hasil model.
  * **Jupyter Notebook:** Sebagai environment untuk pengembangan dan analisis interaktif.


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


## 🤝 Kontribusi

Kontribusi untuk pengembangan proyek ini sangat diterima. Jika Anda ingin berkontribusi, silakan lakukan *fork* pada repositori ini, buat *branch* baru untuk fitur atau perbaikan Anda, dan kirimkan *pull request*.

Terima Kasih