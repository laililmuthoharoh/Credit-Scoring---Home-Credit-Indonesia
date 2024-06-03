# Credit Scoring for Home Credit Indonesia

### Background
Home Credit saat ini sedang menggunakan berbagai macam metode statistik dan Machine Learning untuk membuat prediksi skor kredit. Prediksi skor kredit ini dibuat untuk memastikan pelanggan yang mampu melakukan pelunasan tidak ditolak ketika melakukan pengajuan pinjaman.

### Objective
Masalah yang harus diselesaikan di sini adalah bagaimana caranya agar Home Credit dapat memprediksi dengan benar nasabah-nasabah mana saja yang nantinya akan diberikan pinjaman. Untuk menyelesaikan masalah ini, dapat dilakukan pemodelan klasifikasi dengan machine learning dengan tujuan memprediksi klien mana yang dapat melakukan pelunasan pinjaman dengan baik. Pemodelan ini dilakukan dengan memanfaatkan data klien sebagai input, dengan output berupa variabel yang menjelaskan status kelancaran klien dalam melakukan pembayaran cicilan.

Ada beberapa pemodelan machine learning yang bisa dimanfaatkan untuk penyelesaian masalah ini. Diantaranya adalah pemodelan Logistic Regression dan pemodelan dengan Random Forest.

Selanjutnya, akan dilakukan klasifikasi menggunakan dua metode ini. Kemudian dibandingkan hasilnya dan diambil metode yang terbaik.

### Dataset
Dataset yang digunakan merupakan data klien dari Home Credit. Data memiliki total 307511 id klien dengan 121 kolom fitur dan 1 kolom output. 

### Machine Learning Modeling
Karena pediksi skor kredit ini dibuat untuk memastikan pelanggan yang mampu melakukan pelunasan tidak ditolak ketika melakukan pengajuan pinjaman, maka kita perlu fokus pada nilai recall.

Berikut diberikan perbandingan nilainya pada data test:

`Logistic Regression (Oversampling): 0.7`

`Random Forest (Oversampling): 0.92`

`Logistic Regression (Undersampling): 0.68`

`Random Forest (Undersampling): 0.63`

Dapat disimpulkan berdasarkan nilai recallnya, maka model terbaik adalah dari Random Forest dengan data oversampling.



