# BIG DATA PROGRAMMING

**Nama:** Alya Maura Raditha  
**NIM:** 52240003  
**Program Studi:** Sains Data  
**Institusi:** Institut Teknologi Sains Bandung (ITSB)

## Deskripsi

Repository ini berisi dokumentasi pengerjaan tugas dan praktikum mata kuliah **Big Data Programming** menggunakan Apache Spark dan PySpark di lingkungan Google Colab.

Pengerjaan mencakup pemrosesan data berskala besar menggunakan pendekatan Resilient Distributed Dataset (RDD), Spark DataFrame API, Spark SQL, serta penerapan teknik optimasi dan analisis data terdistribusi.

## Daftar Penugasan

### 1. PySpark RDD – Online Retail Dataset

**File:** `BIG-DATA1-ALYA MAURA RADITHA.ipynb`

Penugasan pertama berfokus pada pemrosesan data transaksi retail menggunakan PySpark RDD dengan dataset Online Retail.

**Materi dan analisis yang dikerjakan:**

- Pengambilan dan pembersihan dataset.
- Inisialisasi SparkContext dan pembentukan RDD.
- Transformasi RDD menggunakan `filter()` dan `map()`.
- Agregasi transaksi menggunakan `reduceByKey()` dan sorting.
- Optimasi pemrosesan menggunakan caching dan persistence.
- Analisis produk terlaris.
- Analisis pelanggan dengan nilai transaksi tertinggi.
- Identifikasi transaksi pembatalan dan retur.
- Eksperimen jumlah partisi dan perbandingan performa `reduceByKey()` dengan `groupByKey()`.
- Analisis jam sibuk transaksi.
- Analisis produk bertema HEART.
- Operasi himpunan menggunakan `subtract()` untuk membandingkan produk Germany dan France.

**Dataset:** Online Retail Dataset (`OnlineRetail.csv`).

### 2. PySpark DataFrame API & Spark SQL – NYC Yellow Taxi Dataset

**File:** `BIG-DATA2-ALYA MAURA RADITHA.ipynb`

Penugasan kedua berfokus pada pengolahan dan analisis data perjalanan taksi New York menggunakan PySpark DataFrame API dan Spark SQL.

**Materi dan analisis yang dikerjakan:**

- Pengambilan dataset dan ingestion menggunakan explicit schema.
- Pembersihan data dan feature engineering.
- Agregasi data menggunakan Spark DataFrame API.
- Analisis jam sibuk berdasarkan waktu penjemputan.
- Analisis durasi perjalanan dan tarif berdasarkan jumlah penumpang.
- Segmentasi jarak perjalanan menggunakan `CASE WHEN` pada Spark SQL.
- Analisis metode pembayaran dan persentase tip.
- Penerapan Window Function menggunakan `dense_rank()`.
- Ekspor hasil agregasi ke format Parquet dengan kompresi Snappy.

**Dataset:** NYC Yellow Taxi Trips (`yellow_tripdata_2015-01.csv`).

## Teknologi dan Tools

| Teknologi | Penggunaan |
|---|---|
| Python | Bahasa pemrograman utama |
| Apache Spark | Pemrosesan data terdistribusi |
| PySpark RDD | Transformasi dan agregasi data |
| Spark DataFrame API | Manipulasi dan analisis data |
| Spark SQL | Analisis menggunakan kueri SQL |
| Google Colab | Lingkungan eksekusi notebook |
| Google Drive | Penyimpanan dan pengambilan dataset |
| Parquet | Penyimpanan data terstruktur |
| TXT | Dokumentasi hasil eksekusi |

## Struktur Repository

```text
BIG-DATA-PROGRAMMING/
│
├── BIG-DATA1-ALYA MAURA RADITHA.ipynb
├── BIG-DATA2-ALYA MAURA RADITHA.ipynb
│
└── BIG DATA PROGRAMMING_ALYA MAURA RADITHA_52240003.zip
    ├── BIG-DATA-1.ipynb - Colab.pdf
    ├── BIG-DATA-2.ipynb - Colab.pdf
    ├── output_1.txt
    └── output_2.txt
```

## Cara Menjalankan

Notebook dikerjakan menggunakan Google Colab dengan PySpark.

1. Buka file notebook (`.ipynb`) menggunakan Google Colab.
2. Hubungkan Google Drive melalui Google Colab.
3. Siapkan dataset sesuai nama dan lokasi yang ditentukan dalam notebook:
   - `OnlineRetail.csv`
   - `yellow_tripdata_2015-01.csv`
4. Jalankan setiap cell secara berurutan dari awal hingga akhir.
5. Perhatikan hasil pemrosesan, tabel, dan interpretasi analisis pada setiap bagian.
6. Hasil eksekusi dapat dilihat pada file `output_1.txt` dan `output_2.txt` yang tersedia dalam arsip ZIP.

**Environment:** Google Colab, Python 3.13.18, PySpark 3.5.3.

## Hasil Pengerjaan

Kedua penugasan menghasilkan analisis data terdistribusi dengan pendekatan yang berbeda:

- **Penugasan 1:** Mengolah dataset Online Retail sebanyak 541.909 record mentah, dengan 406.829 record tersisa setelah pembersihan.
- **Penugasan 2:** Mengolah dataset NYC Yellow Taxi sebanyak 12.748.986 record mentah, dengan 12.666.418 record tersisa setelah pembersihan.

Setiap notebook dilengkapi dengan hasil eksekusi, interpretasi temuan, serta evaluasi terhadap hasil analisis yang diperoleh.

---

**Course:** Big Data Programming  
**Student:** Alya Maura Raditha  
**NIM:** 52240003  
**Program:** Data Science – Institut Teknologi Sains Bandung (ITSB)
