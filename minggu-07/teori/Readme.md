# Kelas
    Kelas menyediakan cara menggabungkan data dan fungsionalitas bersama. Membuat kelas baru menciptakan tipe objek baru, memungkinkan instance baru dari tipe itu dibuat. Setiap instance kelas dapat memiliki atribut yang melekat padanya untuk mempertahankan negaranya. Instance kelas juga dapat memiliki metode (ditentukan oleh kelasnya) untuk memodifikasi kondisinya.
    Kelas Python menyediakan semua fitur standar Pemrograman Berorientasi Objek: mekanisme pewarisan kelas memungkinkan beberapa kelas dasar, kelas turunan dapat menimpa metode apa pun dari kelas dasar atau kelasnya, dan metode dapat memanggil metode kelas dasar dengan nama yang sama . Objek dapat berisi jumlah dan jenis data yang berubah-ubah. Seperti halnya untuk modul, kelas mengambil bagian dari sifat dinamis Python: mereka dibuat pada saat runtime, dan dapat dimodifikasi lebih lanjut setelah pembuatan.
## A Word About Names and Objects
    * Objek memiliki individualitas, dan banyak nama (dalam berbagai lingkup) dapat terikat ke objek yang sama.Ini dikenal sebagai aliasing dalam bahasa lain. Ini biasanya tidak dihargai pada pandangan pertama pada Python, dan dapat diabaikan dengan aman ketika berhadapan dengan tipe dasar yang tidak berubah (angka, string, tupel). 
## Python Scopes and Namespaces
    * Namespace adalah pemetaan dari nama ke objek. Sebagian besar ruang nama saat ini diimplementasikan sebagai kamus Python, tetapi itu biasanya tidak terlihat dengan cara apa pun (kecuali untuk kinerja), dan itu mungkin berubah di masa depan.
    * Scopes adalah wilayah tekstual dari program Python di mana namespace dapat diakses secara langsung. "Dapat diakses secara langsung" di sini berarti bahwa referensi yang tidak memenuhi syarat untuk suatu nama berusaha menemukan nama tersebut di namespace.
## A First Look at Classes
    Kelas memperkenalkan sedikit sintaks baru, tiga tipe objek baru, dan beberapa semantik baru. 
    * Sintaks Definisi kelas : Definisi kelas, seperti definisi fungsi (pernyataan def ) harus dieksekusi sebelum mereka memiliki efek.
    * Objek Kelas : Objek kelas mendukung dua jenis operasi: referensi atribut dan instantiasi.
    * Onjeks instans : Satu-satunya operasi yang dipahami oleh objek instan adalah referensi atribut. Ada dua jenis nama atribut yang valid: atribut data dan metode.
    * Objek Metode 
    * Variabel kelas dan instans : Secara umum, variabel instance adalah untuk data unik untuk setiap instance dan variabel kelas adalah untuk atribut dan metode yang dibagikan oleh semua instance kelas.
## Random Remarks
    Jika nama atribut yang sama muncul di kedua instance dan di kelas, maka pencarian atribut memprioritaskan instance.
## Inheritance
    Nama BaseClassName harus didefinisikan dalam lingkup yang berisi definisi kelas turunan. Di tempat nama kelas dasar, ekspresi sewenang-wenang lainnya juga diperbolehkan. Ini bisa berguna, misalnya, ketika kelas dasar didefinisikan dalam modul lain.
## Private Variables
    Variabel instance "Privat" yang tidak dapat diakses kecuali dari dalam suatu objek tidak ada dalam Python. Namun, ada konvensi yang diikuti oleh sebagian besar kode Python: nama diawali dengan garis bawah (misalnya _spam ) harus diperlakukan sebagai bagian non-publik dari API (apakah itu fungsi, metode atau anggota data) .
## Odds and Ends
    Sepotong kode Python yang mengharapkan tipe data abstrak tertentu sering dapat dilewatkan kelas yang mengemulasi metode tipe data itu sebagai gantinya.
## Iterators
    Fungsi iter() berfungsi menghasilkan iterator dari suatu objek. Fungsi ini menciptakan sebuah objek yang bisa di iterasikan satu persatu elemen.
## Generators
    Generator adalah alat sederhana dan kuat untuk membuat iterator. Mereka ditulis seperti fungsi biasa tetapi menggunakan pernyataan yield setiap kali mereka ingin mengembalikan data. Setiap kali next() dipanggil, generator melanjutkan di tempat yang ditinggalkannya (ia mengingat semua nilai data dan pernyataan mana yang terakhir dieksekusi).
## Ekspresi Generator
    Beberapa generator sederhana dapat dikodekan secara ringkas sebagai ekspresi menggunakan sintaksis yang mirip dengan pemahaman daftar tetapi dengan tanda kurung alih-alih tanda kurung siku. Ungkapan-ungkapan ini dirancang untuk situasi di mana generator digunakan segera oleh fungsi penutup. Ekspresi generator lebih kompak tetapi kurang fleksibel daripada definisi generator penuh dan cenderung lebih ramah memori daripada pemahaman daftar setara.