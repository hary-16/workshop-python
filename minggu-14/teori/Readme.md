# An introduction to machine learning with scikit-learn

## Memuat Contoh Dataset
* scikit-learn dilengkapi dengan beberapa dataset standar, misalnya dataset iris dan digit untuk klasifikasi dan dataset diabetes untuk regresi.
* Dataset adalah objek seperti kamus yang menampung semua data dan beberapa metadata tentang data. Data ini disimpan dalam anggota .data , Yang merupakan array n_samples, n_features .

## Belajar Memprediksi
* Dalam kasus dataset digit, tugasnya adalah memprediksi, diberikan gambar, digit mana yang diwakilinya. 
* Dalam scikit-learn, penduga untuk klasifikasi adalah objek Python yang mengimplementasikan metode fit(X, y) dan predict(T).

## Model persistence
* Dimungkinkan untuk menyimpan model di scikit-learn dengan menggunakan model persistensi built-in Python

## Konvensi
* scikit-learn estimators mengikuti aturan tertentu untuk membuat perilakunya lebih prediktif.
* predict() pertama mengembalikan array integer, karena iris.target (array integer) digunakan fit . iris.target_names kedua predict() mengembalikan array string, karena iris.target_names cocok.
