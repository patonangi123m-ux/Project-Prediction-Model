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

# Kesimpulan
Dari semua model, rata-rata memiliki accuracy di atas 60% namun memiliki recall di bawah 40%. Artinya, masih banyak nasabah yang sebenarnya berpotensi gagal bayar namun diprediksi tidak akan gagal bayar. Sehingga bisa disampaikan bahwa dalam iterasi pembangunan model kali ini, objektif yang diinginkan masih belum dapat tercapai.

Solusi pengembangan kedepannya yang bisa dilakukan di antaranya:
1. Memperbanyak sample (jumlah nasabah dgn asumsi dataset yang tersedia saat ini bukan total populasi nasabah)
2. Melakukan oversampling terhadap kelas minoritas (gagal bayar) agar pembangunan model tidak bias
3. Memperluas horizon waktu
4. Mencoba variasi variabel lainnya (menambah variabel baru, atau membuang variabel yang memiliki nilai importance rendah pada hasil terakhir)
5. Mencoba memperluas kombinasi hyperparameter dalam pembangunan model
6. Mencoba algoritma supervised machine learning lainnya
