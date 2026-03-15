# Project-Prediction-Model
Membuat Model Prediksi Pelanggan Gagal Bayar Kartu Kredit

# Problem Statement
Kekhawatiran adanya keterlambatan pembayaran kartu kredit pada FinanKu yang akan merugikan bisnis. Sehingga orang-orang yang memiliki potensi untuk mengalami keterlambatan bayar bisa diprediksi lebih cepat untuk menentukan strategi yang sesuai dalam menghadapi kondisi di masa mendatang.

# Objective
Membuat sebuah model yang dapat memprediksi setidaknya 60% dari pelanggan yang akan mengalami telat bayar kartu kredit [Accuracy & Recall di atas 60%]

# Variabel yang tersedia
Dari dataset yang dimiliki terdapat beberapa data yang tersedia:

1. Customer ID: Unique ID Customer
2. Branch: Lokasi Cabang Nasabah Terdaftar
3. City: Lokasi Kota Nasabah Terdaftar
4. Age: Umur Nasabah Pada Periode Observasi
5. Avg. Annual Income/Month: Rata-rata penghasilan nasabah dalam satu tahun
6. Balance (Q1-Q4): Saldo mengendap yang dimiliki nasabah di akhir kuartal
7. Num of Products (Q1-Q4): Jumlah kepemilikan produk nasabah di akhir kuartal
8. HasCrCard (Q1-Q4): Status kepemilikan produk kartu kredit nasabah di akhir kuartal
9. Active Member (Q1-Q4): Status keaktifan nasabah
10. Unpaid Tagging: Status nasabah gagal bayar

# Eksperimen
Periode Tinjauan:
1. Nasabah direview selama satu tahun terakhir
2. Nasabah direview selama 6 bulan terakhir

Penyesuaian Variabel:
1. Balance dilihat dari rata-rata selama horizon waktu & dilihat perubahan pada akhir tinjauan dan awal tinjauan
2. Melihat kepemilikan jumlah produk dari rata-rata, maksimum, dan minimum pada periode tinjauan
3. Status keaktifan nasabah dilihat dalam bentuk bulan
