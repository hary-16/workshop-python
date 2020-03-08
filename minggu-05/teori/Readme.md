# Input dan Output
## Pemformatan Output yang lebih menarik

**Ketika tidak membutuhkan output mewah tetapi hanya ingin tampilan cepat dari beberapa variabel untuk keperluan debugging, Dapat mengonversi nilai apa pun menjadi string dengan fungsi repr() atau str().Fungsi str() dimaksudkan untuk mengembalikan representasi nilai-nilai yang terbaca oleh manusia, sementara repr() dimaksudkan untuk menghasilkan representasi yang dapat dibaca oleh penerjemah. 
**Modul string berisi kelas Template yang menawarkan cara lain untuk mengganti nilai menjadi string, menggunakan placeholder seperti $x dan menggantinya dengan nilai-nilai dari kamus, tetapi menawarkan kontrol format yang jauh lebih sedikit. 

## Membaca dan Menulis File

** open() berfungsi untuk mengembalikan objek file , dan paling umum digunakan dengan dua argumen: open(filename, mode) .
** Keuntungan menggunakan kata kunci with saat menangani objek file adalah file ditutup dengan benar setelah suite-nya selesai, bahkan jika suatu pengecualian muncul di beberapa titik.Jika tidak menggunakan kata kunci with , maka harus memanggil f.close() untuk menutup file dan segera membebaskan semua sumber daya sistem yang digunakan olehnya.
** Untuk membaca konten file, panggil f.read(size) , yang membaca beberapa kuantitas data dan mengembalikannya sebagai string (dalam mode teks) atau objek byte (dalam mode biner).
** f.readline() digunakan untuk membaca satu baris dari file,Jika ingin membaca semua baris file dalam daftar, dapat menggunakan list(f) atau f.readlines() .
** f.write(string) menulis konten string ke file, mengembalikan jumlah karakter yang ditulis.
** f.tell() mengembalikan integer yang memberikan posisi objek file saat ini dalam file yang direpresentasikan sebagai jumlah byte dari awal file ketika dalam mode biner dan angka buram ketika dalam mode teks.
