# ☕ Dashboard Cafe Semarang

Dashboard analisis penjualan **KM02 Coffee and Working Space** menggunakan pendekatan **Business Intelligence** dengan implementasi **Data Warehouse**, **ETL (Extract, Transform, Load)**, **OLAP**, dan **Microsoft Power BI** untuk menghasilkan insight bisnis dari data transaksi penjualan.

---

# 📖 Project Overview

Project ini bertujuan menganalisis data transaksi penjualan Cafe KM02 Coffee and Working Space selama **Juni 2023**. Dataset berisi **2.762 transaksi** dengan **25 atribut** yang mencakup informasi produk, waktu transaksi, metode pembayaran, hingga nilai penjualan.

Melalui penerapan Data Warehouse dan dashboard interaktif, project ini membantu dalam memonitor performa penjualan serta mendukung pengambilan keputusan berbasis data.

---

# 🎯 Objectives

- Merancang Data Warehouse menggunakan Star Schema.
- Melakukan proses ETL terhadap data transaksi.
- Membangun dashboard interaktif menggunakan Microsoft Power BI.
- Melakukan analisis OLAP terhadap data penjualan.
- Menyediakan insight bisnis untuk mendukung pengambilan keputusan.

---

# 🛠️ Technologies

- Microsoft Power BI
- Power Query
- Python
- Pandas
- Draw.io
- Microsoft Excel / CSV

---

# 🗄️ Data Warehouse

Project ini menggunakan **Star Schema** sebagai model Data Warehouse.

## Fact Table

### Fact_Penjualan

Berisi seluruh data transaksi penjualan seperti:

- Receipt Number
- Quantity
- Gross Sales
- Discount
- Refunds
- Net Sales
- Tax
- Gratuity

---

## Dimension Tables

### 📅 Dim_Waktu

- Date_ID
- Time_ID
- Tanggal
- Bulan
- Tahun
- Jam
- Menit
- Detik

### 🍽️ Dim_Produk

- SKU
- Category
- Brand
- Items
- Variant
- Modifier Applied

### 👨‍💼 Dim_Karyawan

- Karyawan_ID
- Served_By
- Collected_By

### 💳 Dim_Pembayaran

- Payment_Method_ID
- Payment_Method
- Event_Type

### 🛍️ Dim_Sales

- Sales_Type_ID
- Sales_Type

---

# ⭐ Star Schema

Diagram berikut menunjukkan hubungan antara tabel fakta dan tabel dimensi yang digunakan dalam Data Warehouse.

<p align="center">
  <img src="Warehouse.drawio.png" width="850">
</p>

---

# 🔄 ETL Process

Tahapan ETL yang dilakukan meliputi:

### Extract

- Mengimpor dataset transaksi penjualan.
- Membaca data dari file CSV.

### Transform

- Membersihkan data duplikat.
- Menstandarkan nilai Sales Type.
- Mengelompokkan metode pembayaran.
- Menentukan waktu puncak penjualan.
- Membentuk atribut dimensi waktu.

### Load

- Memuat data hasil transformasi ke Microsoft Power BI.

---

# 📊 Dashboard Features

Dashboard Power BI menyajikan beberapa visualisasi, antara lain:

- Total Sales
- Total Revenue
- Total Transactions
- Best Selling Products
- Sales Trend
- Peak Sales Time
- Sales by Category
- Sales by Sales Type
- Sales by Payment Method
- Discount Analysis

---

# 📈 Business Questions

Dashboard dikembangkan untuk menjawab beberapa pertanyaan bisnis berikut.

- Produk apa yang memiliki penjualan tertinggi?
- Kapan waktu puncak penjualan terjadi?
- Bagaimana distribusi penjualan berdasarkan Sales Type?
- Bagaimana pengaruh diskon terhadap penjualan?
- Metode pembayaran apa yang paling sering digunakan?

---

#
# 📄 Documentation

Repository ini juga dilengkapi dengan laporan analisis Business Intelligence yang menjelaskan:

- Perancangan Data Warehouse
- Proses ETL
- Analisis OLAP
- Dashboard Power BI
- Insight Bisnis

---

# 💡 Business Insights

Melalui dashboard ini, pengguna dapat:

- Mengidentifikasi produk dengan penjualan tertinggi.
- Mengetahui waktu puncak transaksi.
- Menganalisis distribusi penjualan berdasarkan kategori dan jenis penjualan.
- Mengevaluasi efektivitas program diskon.
- Menganalisis preferensi metode pembayaran pelanggan.

---

# 👨‍💻 Author

**Reza Dwi Puspita**

Universitas Islam Indonesia

---

# 📜 License

Project ini dibuat sebagai portofolio dalam bidang **Business Intelligence**, **Data Warehouse**, **ETL**, dan **Power BI**.
