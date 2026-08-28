# 📊 Global Superstore Sales & Profitability Analysis Dashboard

## 📌 Project Overview

Proyek ini merupakan latihan analisis data penjualan dan profitabilitas menggunakan **Microsoft Excel**. Saya menganalisis data transaksi Global Superstore selama periode **2011–2014**, dengan total **51,284 records** setelah proses data cleaning.

Dalam proyek ini, saya membuat dashboard interaktif untuk melihat hubungan antara **Sales, Profit, Discount, Category, dan Sub-Category**.

Analisis digunakan untuk melihat pola penjualan dan profit dari waktu ke waktu, membandingkan profitabilitas antar-sub-kategori produk, serta mengeksplorasi hubungan antara tingkat diskon dan profit berdasarkan data yang tersedia.

---

## 🗂️ Dataset

- **Dataset:** Global Superstore Dataset
- **Source:** Kaggle
- **Publisher:** Fatih İlhan
- **Period:** 2011–2014
- **Records:** 51,284

📎 **Dataset Source:**  
[Global Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/fatihilhan/global-superstore-dataset)

---

## 🛠️ Data Preparation & Analysis

Beberapa proses yang saya lakukan dalam proyek ini meliputi:

### Data Preparation

- Memeriksa data kosong pada variabel yang digunakan dalam analisis
- Menghapus 6 baris data kosong sehingga jumlah data yang digunakan menjadi **51,284 records**
- Memeriksa dan menyesuaikan format data
- Menerapkan custom number formatting untuk meningkatkan keterbacaan nilai Sales dan Profit

### Data Transformation

- Membuat **Group Sales** untuk mengelompokkan nilai transaksi ke dalam beberapa rentang
- Membuat **Group Discount** untuk mengelompokkan tingkat diskon ke dalam beberapa interval persentase
- Mengekstrak informasi **Month** dari kolom Order Date untuk mendukung analisis bulanan

### Analysis & Excel Features

- Menggunakan **PivotTables** untuk membantu proses analisis
- Membuat **Slicers** untuk memfilter data berdasarkan Year, Month, Segment, dan Market
- Membuat KPI Summary
- Membandingkan Sales dan Profit berdasarkan bulan
- Menganalisis hubungan antara tingkat Discount dan Profit
- Membandingkan profitabilitas antar-sub-category produk
- Membuat dashboard interaktif menggunakan Microsoft Excel

---

# 📈 Dashboard Highlights & Key Insights

## 1️⃣ Monthly Sales & Profit Trend

Combo Chart digunakan untuk membandingkan perubahan **Sales dan Profit** berdasarkan bulan.

### 🔍 Key Insight

Berdasarkan hasil analisis, Sales dan Profit menunjukkan peningkatan pada beberapa bulan menjelang akhir tahun.

- **November** mencatat Sales sebesar **$1.55M** dengan Profit sebesar **$175.4K**
- **Desember** mencatat Sales sebesar **$1.58M** dengan Profit sebesar **$170.6K**
- **Juli** mencatat Sales sebesar **$749K**
- Sales kembali meningkat pada **Agustus** menjadi **$1.29M**

Berdasarkan data yang tersedia, November dan Desember memiliki nilai Sales tertinggi dibandingkan bulan lainnya.

---

## 2️⃣ Discount & Profit Analysis

Analisis ini membandingkan tingkat Discount dengan Profit yang dihasilkan berdasarkan kelompok diskon.

### 🔍 Key Insight

Berdasarkan hasil analisis:

- Kelompok diskon **0–10%** menghasilkan Profit terbesar, yaitu lebih dari **$2.11M**
- Kelompok transaksi dengan Discount di atas **20%** menunjukkan Profit negatif dalam data yang dianalisis
- Kerugian terbesar tercatat pada kelompok Discount **51–60%**, yaitu sekitar **-$214.8K**
- Kelompok Discount **71–80%** juga mencatat Profit negatif sebesar sekitar **-$197.5K**

Hasil ini menunjukkan bahwa pada dataset yang dianalisis, tingkat diskon yang lebih tinggi tidak selalu menghasilkan profit yang lebih tinggi.

---

## 3️⃣ Sub-Category Profitability

Bar Chart digunakan untuk membandingkan Profit antar-sub-category produk.

### 🔍 Key Insight

Berdasarkan data yang tersedia:

- **Copiers** memiliki Profit tertinggi sebesar **$258.6K**
- **Phones** memiliki Profit sebesar **$216.7K**
- **Tables** mencatat Profit negatif terbesar sebesar **-$64.1K**

Perbandingan ini membantu mengidentifikasi sub-category dengan kontribusi Profit positif dan sub-category yang menghasilkan Profit negatif selama periode analisis.

---

## 💡 Analytical Considerations

Berdasarkan hasil analisis, terdapat beberapa hal yang dapat menjadi pertimbangan untuk analisis lebih lanjut:

- Hubungan antara Discount dan Profit dapat dianalisis lebih lanjut sebelum menentukan kebijakan diskon.
- Sub-category dengan Profit negatif, seperti **Tables**, dapat dievaluasi lebih lanjut untuk memahami faktor yang memengaruhi profitabilitasnya.
- Pola peningkatan Sales pada beberapa bulan menjelang akhir tahun dapat digunakan sebagai dasar untuk mengeksplorasi pola musiman dalam data.

> **Note:** Temuan dalam proyek ini didasarkan pada data dan variabel yang tersedia dalam dataset. Hasil analisis tidak digunakan sebagai dasar untuk menentukan keputusan bisnis secara langsung.

---

# 🖼️ Dashboard Preview

![Global Superstore Sales Dashboard Preview](Sales%20Dashboard%20Image.jpeg)

📄 **[View Full Dashboard in High-Resolution PDF](./Sales%20Dashboard%20PDF.pdf)**

---

# 📁 Workbook Structure

**Sales Data:** Berisi data transaksi yang digunakan dalam proses analisis.

**Data Cleaning:** Digunakan untuk proses pemeriksaan dan pengolahan data sebelum analisis.

**Staging KPI:** Berisi PivotTables dan perhitungan pendukung yang digunakan dalam dashboard.

**Dashboard:** Berisi hasil akhir dashboard, termasuk KPI, charts, dan interactive slicers.

📄 **Main File:**  
`Sales_Performance_Analysis_Dashboard.xlsx`

---

# 🧰 Tools & Skills Demonstrated

**Tool Used:** Microsoft Excel

**Skills & Techniques:**

- Data Cleaning
- Data Preparation
- Data Transformation
- Date Manipulation
- Nested IF
- PivotTables
- PivotCharts
- Interactive Slicers
- Data Visualization
- Sales Analysis
- Profitability Analysis
- Trend Analysis
- Dashboard Development

---

# 🎯 Project Takeaways

Melalui proyek ini, saya berlatih menganalisis data penjualan dan profitabilitas serta mengubah hasil analisis menjadi dashboard menggunakan Microsoft Excel. 
Proyek ini juga membantu saya memahami proses analisis data secara lebih praktis, mulai dari:

**Raw Data → Data Preparation → Analysis → Visualization → Dashboard Development**

---

# 👤 Author

**Alena Mansika**

- 💻 **GitHub:** [@alenamansika](https://github.com/alenamansika)
- 💼 **LinkedIn:** [Alena Mansika](https://www.linkedin.com/in/alenamansika)
