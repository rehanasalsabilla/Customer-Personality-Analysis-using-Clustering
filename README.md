# 🧠 Customer Personality Analysis using Clustering

Proyek ini bertujuan untuk melakukan **Customer Segmentation** menggunakan algoritma **K-Means Clustering**.  
Dengan mengelompokkan pelanggan berdasarkan karakteristik dan perilaku mereka, perusahaan dapat memahami profil pelanggan, menyusun strategi pemasaran yang lebih tepat sasaran, serta meningkatkan retensi pelanggan.

---

## 📊 Deskripsi Proyek

**Customer Personality Analysis** adalah proses memahami perilaku, preferensi, dan karakteristik pelanggan agar perusahaan dapat membuat keputusan yang lebih berbasis data.  
Alih-alih memasarkan produk ke semua pelanggan secara umum, segmentasi pelanggan membantu perusahaan fokus pada **kelompok pelanggan yang paling potensial**.

Dalam proyek ini dilakukan beberapa tahap utama:
- 🧩 Eksplorasi data (EDA)  
- 🧹 Pembersihan dan normalisasi data  
- 📉 Reduksi dimensi menggunakan **PCA**  
- 🤖 Pengelompokan pelanggan dengan **K-Means Clustering**  
- 📊 Visualisasi hasil dan interpretasi tiap segmen pelanggan  

---

## 🧾 Dataset

**Dataset:** `customer_segmentation.csv`  

Dataset ini berisi informasi karakteristik pelanggan seperti:
- 👤 Umur  
- 💰 Pendapatan tahunan  
- 💍 Status pernikahan  
- 🎓 Pendidikan  
- 🛒 Pengeluaran tahunan  
- 🛍️ Kebiasaan pembelian  

> Dataset ini digunakan untuk menemukan pola dan kesamaan di antara pelanggan agar bisa dibagi menjadi beberapa **segmen homogen**.

## ⚙️ Tahapan Analisis

### 1️⃣ Import Library
Menggunakan library utama:
- `pandas`, `numpy` → untuk manipulasi dan analisis data  
- `matplotlib`, `seaborn` → untuk visualisasi data  
- `sklearn` → untuk preprocessing dan penerapan algoritma **K-Means Clustering**

---

### 2️⃣ Data Understanding (EDA)
Tahapan ini bertujuan memahami struktur dan karakteristik dataset:
- Melihat struktur data, tipe variabel, dan **missing values**  
- Menampilkan **statistik deskriptif** untuk memahami distribusi fitur  
- Melakukan **visualisasi hubungan antar fitur** untuk menemukan pola awal  

---

### 3️⃣ Data Preprocessing
Sebelum clustering, dilakukan beberapa langkah persiapan data:
- Mengatasi **missing values** menggunakan `SimpleImputer`  
- Melakukan **standarisasi data** menggunakan `StandardScaler` agar tiap fitur memiliki skala yang seragam  
- Mereduksi dimensi menggunakan **PCA (Principal Component Analysis)** untuk memudahkan visualisasi cluster  

---

### 4️⃣ K-Means Clustering
Langkah utama untuk melakukan segmentasi pelanggan:
- Menentukan jumlah cluster optimal menggunakan **metode Elbow**  
- Mengelompokkan pelanggan menjadi beberapa segmen berdasarkan kesamaan perilaku  
- Menambahkan hasil cluster ke dalam dataframe untuk analisis lebih lanjut  

---

### 5️⃣ Visualisasi & Interpretasi
Menampilkan hasil clustering dalam bentuk **plot 2D (berbasis PCA)** dan menganalisis karakteristik tiap cluster:

| Cluster | Karakteristik Utama |  
|----------|----------------------|  
| **Cluster 0** | Pelanggan berpendapatan tinggi & loyal |  
| **Cluster 1** | Pelanggan baru dengan pengeluaran rendah |  
| **Cluster 2** | Pelanggan muda dengan potensi tinggi |  
| **Cluster 3** | Pelanggan stabil dengan pola pembelian konstan |  

---

## 📊 Hasil Akhir Analisis

Dari hasil penerapan **K-Means Clustering**, diperoleh **4 segmen utama pelanggan** dengan karakteristik dan rekomendasi strategi berikut:

| Cluster | Karakteristik Utama | Rekomendasi Strategi |
|----------|----------------------|----------------------|
| **Cluster 0** | Pendapatan tinggi, pengeluaran besar, loyal | Fokus pada program loyalitas dan rekomendasi produk premium |
| **Cluster 1** | Pendapatan rendah, pembelian jarang | Tawarkan diskon dan promo produk terjangkau |
| **Cluster 2** | Usia muda, pengeluaran sedang, potensial berkembang | Gunakan pendekatan digital marketing (iklan media sosial) |
| **Cluster 3** | Usia menengah, pembelian stabil | Pertahankan kepuasan dan dukungan pelanggan jangka panjang |

📈 Visualisasi hasil menunjukkan **pemisahan yang cukup jelas antar segmen pelanggan**, membuktikan bahwa algoritma **K-Means** berhasil menemukan pola tersembunyi dalam data.

---

## 🏁 Kesimpulan

Proyek **Customer Personality Analysis using Clustering** berhasil:
- Mengidentifikasi empat kelompok pelanggan dengan karakteristik berbeda.  
- Memberikan insight berharga untuk strategi pemasaran yang lebih efektif dan personal.  
- Membuktikan bahwa pendekatan **data-driven segmentation** dapat membantu bisnis memahami pelanggan dengan lebih mendalam.

Dengan hasil ini, perusahaan dapat meningkatkan efisiensi kampanye pemasaran, mengoptimalkan pengalaman pelanggan, serta memperkuat loyalitas jangka panjang.

## 💡 Insight & Manfaat

Dari hasil analisis, perusahaan dapat memperoleh berbagai manfaat strategis, antara lain:

- 🔎 Mengidentifikasi **kelompok pelanggan potensial**.  
- 🎯 Menentukan **strategi pemasaran yang personal dan efisien**.  
- 💸 Mengoptimalkan **alokasi sumber daya promosi**.  
- 🤝 Meningkatkan **retensi pelanggan dan kepuasan** secara keseluruhan.  

---

## 🧰 Tools dan Teknologi

| Kategori | Teknologi |
|-----------|------------|
| **Bahasa Pemrograman** | Python |
| **Analisis Data** | Pandas, NumPy |
| **Visualisasi** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-learn (KMeans, PCA) |
| **Lingkungan Pengembangan** | Jupyter Notebook |

---

## 🧭 Kesimpulan Akhir

Berdasarkan analisis dan hasil clustering yang dilakukan:

- ✅ **K-Means Clustering** berhasil membagi pelanggan menjadi **4 kelompok berbeda** berdasarkan kesamaan karakteristik dan perilaku.  
- 🧠 Setiap cluster memiliki **nilai strategis** yang dapat dimanfaatkan untuk menyusun strategi pemasaran yang lebih efektif dan efisien.  
- 💼 Dengan memahami segmen pelanggan, perusahaan dapat **mengoptimalkan sumber daya pemasaran, meningkatkan loyalitas pelanggan**, serta memperkuat posisi bisnis di pasar.  
- 🤖 Secara keseluruhan, proyek ini menunjukkan bahwa **unsupervised learning (K-Means)** merupakan pendekatan yang efektif dalam **customer segmentation berbasis data**.  

---

