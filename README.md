# OPTIMALISASI-KUALITAS-PENDIDIKAN-DI-SUMATERA

## Medallion Architecture
1. Bronze Layer
   Keberhasilan pengumpulan dan penyimpanan data mentah pendidikan dari berbagai sumber (misalnya BPS, Kemendikbud ) seperti jumlah guru dan peserta didik 2024-2025, Indeks Pembangunan Literasi Masyarakat (IPLM) 2024, dan nilai Ujian Nasional 2018-2019  ke dalam HDFS dalam format aslinya (CSV, JSON, atau file raw). 
3. Silver Layer
   Efektivitas proses pembersihan, validasi (misalnya validasi skema), transformasi (parsing tanggal, penghapusan duplikat, standarisasi data ), dan pengubahan format data menjadi Parquet atau Avro menggunakan Apache Spark untuk ETL dan Apache Hive untuk DDL.  Data yang tersimpan di lapisan ini merupakan data terstruktur yang siap dianalisis, terintegrasi, bersih, dan efisien dalam penyimpanan.
5. Gold Layer
   Keberhasilan agregasi data dan perhitungan metrik kunci untuk menghasilkan insight yang siap digunakan untuk analisis tingkat lanjut.  Data pada lapisan ini disimpan dalam format Parquet atau ORC  dan digunakan untuk kebutuhan laporan, query cepat, dan visualisasi. 

