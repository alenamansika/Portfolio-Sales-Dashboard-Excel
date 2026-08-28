# 📊 Global Superstore Sales & Profitability Analysis (Advanced Excel Dashboard)

## 📌 Project Overview
Proyek ini menganalisis data historis transaksi e-commerce global (**51,284 order**) periode **2011–2014** serta membangun *Executive Interactive Dashboard* di Microsoft Excel untuk membedah tingkat profitabilitas perusahaan. 

Analisis ini melacak tren musiman bulanan (*Seasonality Pattern*), tingkat erosi margin akibat kebijakan diskon (*Discount Erosion*), kontribusi per kategori produk, serta mengidentifikasi sub-kategori pencetak profit utama (*Star Products*) maupun produk yang menggerus margin (*Bleeding Products*).

---

## 🗂️ Data Source & Attribution
* **Dataset:** Global Superstore Sales Dataset (2011–2014)
* **Publisher:** Kaggle (Fatih İlhan)
* **Link Source:** [Kaggle - Global Superstore Dataset](https://www.kaggle.com/datasets/fatihilhan/global-superstore-dataset)

---

## 🛠️ Excel Features & Techniques Used

* **Data Cleaning & Standardisation:**
  * **Missing Value Handling:** Menghapus 6 baris data kosong (*blank rows*) pada variabel finansial utama untuk menjaga integritas data (*data integrity*), menyesuaikan total data transaksi bersih dari 51,290 menjadi **51,284 baris**.
  * **Custom Number Formatting:** Menerapkan pemformatan kustom (`$#,##0,"K"`) dan membagi nilai keuangan menjadi unit desimal **Thousand Dollars ($K)** dan **Million Dollars ($M)** agar tampilan *scorecard* profesional dan mudah dibaca.
* **Feature Engineering:**
  * **Price Binning (`Group Sales`):** Mengelompokkan nilai transaksi ke dalam 6 rentang harga belanja (`$0-$99`, `$100-$299`, dst.) menggunakan rumus `Nested IF`.
  * **Discount Rate Binning (`Group discount`):** Mentransformasi nilai desimal diskon dari kolom `Discount` menjadi interval persentase diskon (`0-10%`, `11-20%`, ..., `81%+`) untuk analisis sensitivitas promosi.
  * **Date Extraction (`Month`):** Mengekstrak nama bulan singkat dari kolom `Order Date` untuk mendukung analisis pola musiman bulanan.
* **Data Staging Architecture & Dynamic Slicers:**
  * **Dedicated Staging Sheet (`Staging KPI`):** Memisahkan area *backend logic* dan *Pivot Tables* dari lembar kerja tampilan utama untuk menjaga kestabilan *file*.
  * **Strategic Slicer Interactivity (`Report Connections`):** Menghubungkan **Slicer Year**, **Month**, **Segment**, dan **Market** secara eksplisit ke seluruh Pivot Table untuk memungkinkan pemfilteran data secara *real-time* tanpa merusak tata letak *grid*.
* **Advanced Charting Mechanics & UI/UX Design:**
  * **Dual-Axis Combo Seasonality Chart:** Menggabungkan batang penjualan bulanan (*Sales*) pada sumbu primer dengan garis keuntungan bersih (*Profit*) pada sumbu sekunder.
  * **Horizontal Bar Chart Sorting:** Memetakan 17 sub-kategori produk secara hierarkis dari pencetak laba tertinggi hingga terendah dengan label nilai yang disesuaikan.
  * **Clean Navy Blue Dashboard Layout:** Menyusun tata letak *Clean Single-Canvas Dashboard* bernuansa *Navy Blue* & *Sage Green* yang pas dalam 1 layar *view* dilengkapi *direct data labels* untuk kemudahan pembacaan eksekutif.

---

## 📈 Interactive Dashboard Showcase

### 1. Pola Musiman Penjualan & Keuntungan Bulanan (Seasonality Analysis)
*Combo Line & Column Chart* deret waktu yang memadukan data volume penjualan bulanan dengan tren laba bersih sepanjang periode 2011–2014.
* **Key Insight:** Penjualan bulanan menunjukkan tren kenaikan yang sangat tajam pada kuartal keempat (Q4). Bulan **November ($1.55M Sales / $175.4K Profit)** dan **Desember ($1.58M Sales / $170.6K Profit)** secara konsisten menjadi puncak tertinggi (*Peak Season*) transaksi tahunan. Terdapat pula penurunan (*dip*) pada bulan **Juli ($749K Sales)** sebelum kembali melonjak di bulan Agustus ($1.29M Sales).

---

### 2. Bahaya Diskon Tersembunyi (Profit Erosion) & Kinerja Sub-Kategori
*Combo Bar-Line Chart* dan *Horizontal Bar Chart* yang memetakan sensitivitas diskon terhadap kerugian margin serta profitabilitas 17 sub-kategori produk.
* **Key Insight:** Transaksi dengan diskon $\le$ 20% menjadi penopang utama profitabilitas bisnis (diskon `0-10%` menyumbang laba terbesar **>$2.11M**). Sebaliknya, diskon di atas 20% secara konsisten menghasilkan **laba bersih negatif (rugi)**, terutama pada kelompok `51-60%` (**-$214.8K**) dan `71-80%` (**-$197.5K**). Di sisi produk, **Copiers ($258.6K)** dan **Phones ($216.7K)** memimpin sebagai pencetak laba terbanyak, sementara sub-kategori **Tables** mencatatkan kerugian paling parah sebesar **-$64.1K**.

---

### 💡 Strategic & Risk Management Recommendation
* **Discount Capping (Prioritas Utama):** Berlakukan batas diskon (*discount cap*) maksimal **20%** untuk transaksi umum guna menghentikan kebocoran profit ratusan ribu dolar secara langsung.
* **Restrukturisasi Kategori Tables:** Lakukan peninjauan ulang terhadap struktur biaya (*cost structure*) produk *Tables*, negosiasi ulang harga beli dari vendor, atau pangkas SKU yang tidak efisien dari katalog.
* **Optimalisasi Inventaris Q4:** Skalakan alokasi pasokan inventaris produk *Copiers* dan *Phones* sejak bulan **Agustus** untuk memaksimalkan lonjakan permintaan akhir tahun.

![Global Superstore Sales Dashboard Preview](Sales%20Dashboard%20Image.jpeg)

📄 **[Download / Lihat Dashboard versi PDF Beresolusi Tinggi](./Sales%20Dashboard%20PDF.pdf)**

---

## 📁 Repository Structure

* `Sales_Performance_Analysis_Dashboard.xlsx` : File kerja utama Excel (mentah, staging KPI, dan dashboard).
* `Sales Dashboard Image.png` : Gambar tangkapan layar visualisasi dashboard beresolusi tinggi.
* `Sales Dashboard PDF.pdf` : Laporan dashboard versi PDF *Executive View*.

---

## 👤 Author
- **GitHub:** [@alenamansika](https://github.com/alenamansika)
- **LinkedIn:** [Alena Mansika](https://www.linkedin.com/in/alenamansika)
