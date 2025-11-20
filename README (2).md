# Analisis Strategi Harga dan Ketersediaan untuk Optimasi Kinerja Airbnb di Bangkok

## 1. Project Overview

Proyek ini bertujuan untuk menganalisis data *listing* Airbnb di Bangkok guna memahami dinamika pasar akomodasi jangka pendek. Analisis ini dilakukan untuk mendukung *City Performance Manager* dalam merumuskan strategi penetapan harga dan pengelolaan ketersediaan yang optimal.

Masalah utama yang diatasi adalah **kompetisi harga yang ketat dan fluktuasi tingkat okupansi** akibat tingginya jumlah *host* dan variasi *listing* di Bangkok.

**Key Objectives:**
* **Menganalisis Keterkaitan Variabel:** Mengidentifikasi hubungan antara harga (`price`), tipe kamar (`room_type`), jumlah ulasan (`number_of_reviews`), dan ketersediaan listing (`availability_365`).
* **Segmentasi Pasar:** Melakukan analisis komparatif performa *listing* antar wilayah (*neighbourhood*) untuk mengetahui area mana yang sensitif harga dan area mana yang berpotensi tinggi.
* **Merumuskan Rekomendasi:** Menyediakan rekomendasi strategis yang *actionable* kepada *host* dan manajemen Airbnb untuk meningkatkan pendapatan dan okupansi.

---

## 2. Data Sources

* **Dataset:** **Airbnb Listings Bangkok** - Data historis detail properti Airbnb di Bangkok, Thailand.
* **Deskripsi Data:** Dataset ini mencakup variabel penting seperti:
    * `price`: Harga sewa per malam.
    * `room_type`: Jenis kamar yang ditawarkan.
    * `neighbourhood`: Area listing berada.
    * `availability_365`: Jumlah hari listing tersedia dalam 365 hari ke depan (nilai rendah = okupansi tinggi).
    * `number_of_reviews`: Indikator permintaan dan kepercayaan tamu.

---

## 3. Technologies Used

* **Programming Language:** Python
* **Libraries:** `Pandas`, `NumPy` (Data Manipulation).
* **Visualization:** `Matplotlib`, `Seaborn`, `Plotly.express` (Eksplorasi dan Visualisasi Data).
* **Statistical Analysis:** `statsmodels.formula.api`, `scipy.stats` (Analisis Regresi dan Statistik Inferensial).
* **Others:** Jupyter Notebook (Lingkungan Pengembangan).

---

## 4. Project Structure
├── README.md          <- Dokumen utama proyek ini.
|
├── data
│   ├── raw            <- File data mentah (Airbnb Listings Bangkok.csv).
│
├── notebooks          <- Jupyter notebooks. 
|   └── Capstone Project Module 2-Brian.ipynb <- Notebook utama berisi EDA, Analisis Statistik, dan Rekomendasi.
├── reports                   <- Hasil analisis.
│   └── figures               <- Grafik dan visualisasi kunci yang dihasilkan.

---

## 5. Summary of Finding

### 5.1 Business Insight (Temuan Kunci)

1.  **Pengaruh Ulasan Terhadap Okupansi:** Jumlah ulasan (`number_of_reviews`) adalah prediktor okupansi (rendahnya `availability_365`) yang paling kuat. Semakin banyak ulasan yang dimiliki listing, semakin rendah ketersediaannya (tinggi okupansi).
2.  **Korelasi Harga dan Ketersediaan:** Terdapat korelasi terbalik (negatif) antara harga (`price`) dan ketersediaan (`availability_365`), yang mengindikasikan bahwa *listing* dengan harga yang terlalu tinggi cenderung memiliki okupansi yang rendah.
3.  **Dinamika Harga Per Wilayah:** Wilayah seperti **Nong Chok** dan **Pathum Wan** menonjol sebagai area premium dengan median harga tertinggi.
4.  **Tipe Kamar Terbaik:** *Entire Home/Apartment* menunjukkan performa harga dan okupansi yang relatif paling stabil dibandingkan *Private Room*.

### 5.2 Actionable Recommendation (Rekomendasi Bisnis)

1.  **Strategi Harga Dinamis Regional:** Terapkan strategi penetapan harga yang disesuaikan secara dinamis dan spesifik untuk setiap wilayah (*neighbourhood*) dan tipe kamar.
2.  **Fokus pada *Review Generation*:** Dorong *host* baru untuk menawarkan promosi harga di awal untuk segera mendapatkan ulasan pertama, karena ulasan adalah investasi jangka panjang untuk okupansi.
3.  **Optimalkan Pasar Transit/Budget:** Berikan panduan penetapan harga khusus untuk *short-stay* traveler.
4.  **Panduan Harga Otomatis:** Kembangkan fitur rekomendasi harga berbasis data *real-time* kepada *host* untuk meminimalkan risiko *overpriced listing*.

---

## 6. Contact

* Name: Brian
* Email: **brian.naufal5420@gmail.com**
* Linkedin: **brian naufal**