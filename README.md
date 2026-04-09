# UTS-Business-Intelligence-Kelompok-17

# 🛍️ Data Warehouse — Customer Shopping Trends

## 👥 Tim

* Shafa Rizqi Nur Wahidah
* Fauzia Inanta Aurelia
* Azhaar Athahiroh
* Alvionej Resna Lawrend

## 📌 Tentang Project

Project ini merupakan implementasi **Data Warehouse** untuk menganalisis tren pembelian pelanggan pada industri retail fashion.

Menggunakan pendekatan:

* ⭐ **Star Schema**
* 🔄 **ETL Process (Python + SQL)**
* 🗄️ **PostgreSQL**
* 📊 **Power BI Dashboard**

---

## 🎯 Tujuan

* Membangun Data Warehouse terstruktur
* Melakukan proses ETL dari dataset CSV
* Menganalisis pola pembelian pelanggan
* Menyajikan insight dalam dashboard interaktif

---

## 🧱 Arsitektur Data Warehouse

Model yang digunakan adalah **Star Schema**:

* **Fact Table**: `fact_sales`
* **Dimension Tables**:

  * `dim_customer`
  * `dim_product`
  * `dim_season`
  * `dim_shipping`

---

## 📊 Dashboard Preview

<img width="1335" height="728" alt="Screenshot 2026-04-09 211550" src="https://github.com/user-attachments/assets/f55968f0-70ec-4b4d-b5d6-e784bdaab781" />

## 📊 Dashboard Insights — Shopping Trends

Bagian ini menjelaskan insight utama yang diperoleh dari dashboard Power BI berdasarkan analisis data transaksi pelanggan.

---

### 🔝 1. KPI Utama

- **Total Revenue: $233K**  
- **Total Transaksi: 3.900**  
- **Average Spend: $59.76**  
- **Average Rating: 3.75 ⭐**

📌 **Insight:**
- Performa bisnis tergolong **stabil** dengan jumlah transaksi yang konsisten  
- Rata-rata pembelian berada di kategori **menengah (medium spending)**  
- Tingkat kepuasan pelanggan cukup baik, namun masih dapat ditingkatkan  

---

### 🛍️ 2. Revenue by Category

- **Clothing** menjadi kontributor terbesar (~44%)
- Diikuti oleh Accessories, Footwear, dan Outerwear

📌 **Insight:**
- Clothing merupakan **core business utama**
- Kategori lain masih memiliki potensi untuk dikembangkan

🎯 **Strategi:**
- Fokus pada promosi kategori utama
- Lakukan **cross-selling** ke kategori lain

---

### 🥇 3. Top 10 Produk

Produk dengan transaksi tertinggi:
- Shirt  
- Sweater  
- Sunglasses  
- Socks  
- Skirt  

📌 **Insight:**
- Produk kebutuhan sehari-hari mendominasi penjualan  
- Distribusi produk cukup merata (tidak ada dominasi ekstrem)

🎯 **Strategi:**
- Bundling produk populer  
- Gunakan produk top sebagai daya tarik utama promosi  

---

### 🌦️ 4. Transaksi Berdasarkan Musim

- **Spring & Fall** → transaksi tertinggi  
- **Summer** → transaksi terendah  

📌 **Insight:**
- Pola pembelian dipengaruhi oleh musim  
- Summer menjadi periode dengan performa terendah  

🎯 **Strategi:**
- Berikan promo khusus saat Summer  
- Maksimalkan campaign pada musim ramai  

---

### 👥 5. Segmentasi Pelanggan (Age Group)

- **Middle Age (40–59)** → segmen terbesar  
- Diikuti oleh Adult  
- Young Adult paling rendah  

📌 **Insight:**
- Target utama saat ini adalah pelanggan usia menengah  
- Segmen usia muda belum optimal  

🎯 **Strategi:**
- Campaign khusus untuk Gen Z / Young Adult  
- Produk lebih trend-oriented  

---

### 💳 6. Payment Method

Metode pembayaran:
- PayPal  
- Cash  
- Credit Card  
- Venmo  
- Bank Transfer  

📌 **Insight:**
- Distribusi penggunaan metode pembayaran relatif **seimbang**  
- Menunjukkan fleksibilitas sistem pembayaran  

🎯 **Strategi:**
- Tambahkan promo berdasarkan metode pembayaran (cashback, dll)

---

### 👤 7. Subscriber vs Non-Subscriber

- Non-subscriber mendominasi (~90%+)  
- Subscriber masih sangat rendah  

📌 **Insight (KRITIS 🚨):**
> Program subscription belum efektif dalam menarik pelanggan

🎯 **Strategi:**
- Tingkatkan benefit subscription:
  - Diskon eksklusif  
  - Free shipping  
  - Loyalty program  

---

## 🎯 Kesimpulan

Secara keseluruhan, bisnis menunjukkan performa yang stabil dengan kontribusi utama dari kategori Clothing dan segmen pelanggan usia Middle Age.

Namun, terdapat beberapa peluang pengembangan:
- Meningkatkan jumlah subscriber (customer retention)
- Mengoptimalkan penjualan di musim rendah (Summer)
- Mengembangkan segmen pelanggan usia muda

---

💡 Insight ini dapat digunakan sebagai dasar pengambilan keputusan strategis untuk meningkatkan performa bisnis ke depannya.
---

## 💰 KPI Utama

| KPI             | Nilai    |
| --------------- | -------- |
| Total Revenue   | $233,081 |
| Total Transaksi | 3,900    |
| Avg Spend       | $59.76   |
| Avg Rating      | 3.75     |

---

## 🔍 Key Insights

* 🛍️ **Clothing** adalah kategori dengan revenue tertinggi (~44%)
* 📈 **Middle Age** adalah segmen pelanggan terbesar
* ☀️ **Summer** memiliki performa terendah (peluang promosi)
* 👤 **Non-subscriber mendominasi (73%)**

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy)
* PostgreSQL
* pgAdmin
* Power BI
* Google Colab

---

## 📁 Struktur Project

```
shopping-dw-project/
│
├── dataset/
├── notebooks/
├── sql/
├── report/
└── README.md
```

---

## 🔄 ETL Process

1. Extract data dari CSV
2. Data cleaning & transformasi (Python)
3. Generate SQL
4. Load ke PostgreSQL
5. Visualisasi di Power BI

---

## 🚀 Cara Menjalankan

### 1. Clone repo

```bash
git clone https://github.com/USERNAME/shopping-dw-project.git
cd shopping-dw-project
```

### 2. Install library

```bash
pip install pandas numpy sqlalchemy psycopg2-binary
```

### 3. Jalankan SQL

* `create_tables.sql`
* `insert_data.sql`

### 4. Connect Power BI

* Server: `localhost:5432`
* Database: `shopping_dw`

---

## 📊 Dashboard Pages

### 📄 Page 1 — Executive Summary

* KPI
* Revenue by Category
* Top Produk
* Transaksi by Season

### 📄 Page 2 — Customer Segmentation

* Age Group
* Gender
* Subscriber

### 📄 Page 3 — Transaction Analysis

* Payment Method
* Discount Analysis
* Shipping Type

---
