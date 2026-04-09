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
