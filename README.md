# Analisis Korelasi Popularitas Seiyuu dan Anime

Sebuah analisis untuk menguji hubungan antara popularitas seorang **Seiyuu** (pengisi suara) dengan popularitas **Anime** yang dibintanginya, menggunakan data dari MyAnimeList.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📚 Latar Belakang

Di komunitas anime, seringkali ada anggapan bahwa Seiyuu (pengisi suara) terkenal identik dengan anime yang sukses. Proyek ini lahir dari rasa penasaran: **Apakah ada korelasi statistik yang signifikan antara popularitas seorang seiyuu dengan popularitas anime yang mereka perankan?**

Analisis ini bertujuan untuk menjawab pertanyaan tersebut secara kuantitatif dengan mengolah dan memvisualisasikan data yang diambil dari situs **MyAnimeList (MAL)**, salah satu database anime dan manga terbesar di dunia.

---

## 📊 Metodologi

Analisis dilakukan melalui beberapa tahapan utama:

1.  **Pengumpulan Data (Data Scraping/API)**
    Data anime dan seiyuu dikumpulkan dari MyAnimeList. Atribut utama yang diambil meliputi:
    * **Untuk Anime:** Judul, Skor, Peringkat (Rank), Popularitas, dan Jumlah Anggota.
    * **Untuk Seiyuu:** Nama dan Jumlah "Member Favorites".

2.  **Pembersihan dan Pra-pemrosesan Data (Data Cleaning & Preprocessing)**
    Data mentah yang telah dikumpulkan kemudian dibersihkan dari nilai yang hilang (*missing values*), digabungkan, dan distrukturkan ulang agar siap untuk dianalisis.

3.  **Analisis Korelasi (Correlation Analysis)**
    Hubungan antara popularitas seiyuu dan popularitas anime diukur menggunakan metode statistik, seperti **korelasi Pearson**. Metrik yang dibandingkan adalah:
    * `Jumlah Favorites Seiyuu` vs. `Skor Rata-rata Anime`
    * `Jumlah Favorites Seiyuu` vs. `Jumlah Anggota Rata-rata Anime`

4.  **Visualisasi Data (Data Visualization)**
    Hasil analisis disajikan dalam bentuk visual seperti *scatterplot* dan *heatmap* untuk mempermudah interpretasi dan menarik kesimpulan.

---

## ⚙️ Teknologi yang Digunakan

* **Bahasa Pemrograman:** Python
* **Library Analisis Data:**
    * `Pandas`: Untuk manipulasi dan pemrosesan data.
    * `NumPy`: Untuk operasi numerik.
* **Library Visualisasi Data:**
    * `Matplotlib`: Untuk membuat plot dasar.
    * `Seaborn`: Untuk membuat visualisasi statistik yang lebih menarik.
* **Lingkungan Kerja:** Jupyter Notebook
* **Pengambilan Data:** `[Sebutkan library yang Anda gunakan, contoh: Jikanpy, BeautifulSoup, atau Scrapy]`

---

## 🚀 Cara Menjalankan Proyek

Untuk menjalankan analisis ini di lingkungan lokal Anda, ikuti langkah-langkah berikut:

1.  **Clone repository ini:**
    ```bash
    git clone [https://github.com/RaihanSabil/Analisis-Korelasi-Popularitas-Seiyuu-dan-Anime-Berdasarkan-Data-MyAnimeList.git](https://github.com/RaihanSabil/Analisis-Korelasi-Popularitas-Seiyuu-dan-Anime-Berdasarkan-Data-MyAnimeList.git)
    cd Analisis-Korelasi-Popularitas-Seiyuu-dan-Anime-Berdasarkan-Data-MyAnimeList
    ```

2.  **Buat dan aktifkan virtual environment (opsional tapi direkomendasikan):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Untuk Windows: venv\Scripts\activate
    ```

3.  **Instal semua dependensi yang dibutuhkan:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Jalankan Jupyter Notebook:**
    Buka dan jalankan file notebook (`.ipynb`) yang ada di dalam direktori proyek untuk melihat seluruh proses analisis.
    ```bash
    jupyter notebook [nama_file_notebook_anda].ipynb
    ```

---

## 📈 Hasil dan Kesimpulan

`[Di bagian ini, jelaskan secara singkat temuan utama Anda. Ini adalah bagian terpenting!]`

**Contoh:**
Berdasarkan analisis yang telah dilakukan, ditemukan **korelasi positif yang [lemah/sedang/kuat]** antara jumlah *favorites* seorang seiyuu dengan skor rata-rata anime yang dibintanginya. Hal ini mengindikasikan bahwa seiyuu yang lebih populer cenderung terlibat dalam proyek anime yang dinilai lebih tinggi oleh komunitas.

*[Sisipkan gambar visualisasi utama Anda di sini, misalnya scatter plot korelasi]*

Namun, perlu dicatat bahwa korelasi tidak menyiratkan sebab-akibat. Popularitas anime dipengaruhi oleh banyak faktor lain seperti studio, cerita, dan sutradara.

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **Lisensi MIT**. Lihat file `LICENSE` untuk detail lebih lanjut.
