# Error dan Exception

## Kesalahan Sintaksis(Parsing)
* Parser mengulangi baris yang menyinggung dan menampilkan sedikit 'panah' yang menunjuk pada titik paling awal di baris di mana kesalahan terdeteksi. Kesalahan disebabkan oleh (atau setidaknya terdeteksi pada) token sebelum panah.

## Exception
* Kesalahan yang terdeteksi selama eksekusi disebut exception dan tidak berakibat fatal.

## Menangani exception
* Untuk menangangi suatu exception digunakan blok try
* Pernyataan try berfungsi sebagai berikut.
	1. Pertama, klausa coba (pernyataan) antara try dan except kata kunci) dieksekusi.
	2. Jika tidak ada pengecualian terjadi, kecuali klausa dilewati dan eksekusi pernyataan try selesai.
	3. Jika pengecualian terjadi selama eksekusi klausa coba, sisa klausa dilewati. Kemudian jika jenisnya cocok dengan pengecualian yang dinamai dengan kata kunci except , klausa kecuali dijalankan, dan kemudian eksekusi berlanjut setelah pernyataan try .
	4. Jika pengecualian terjadi yang tidak cocok dengan pengecualian yang disebutkan dalam klausa kecuali, itu diteruskan ke pernyataan try luar; jika tidak ada pawang yang ditemukan, itu adalah pengecualian yang tidak tertangani dan eksekusi berhenti dengan pesan seperti yang ditunjukkan di atas.

## Raising Exception
* Pernyataan raise memungkinkan programmer untuk memaksa pengecualian yang ditentukan terjadi.
* rgumen tunggal untuk raise mengindikasikan pengecualian yang akan diajukan. Ini harus berupa instance pengecualian atau kelas pengecualian (kelas yang berasal dari Exception ). Jika kelas pengecualian dilewatkan, itu akan secara implisit dipakai dengan memanggil konstruktornya tanpa argumen

## User-defined Exceptions
* Program dapat memberi nama pengecualian mereka sendiri dengan membuat kelas pengecualian baru.Pengecualian biasanya berasal dari kelas Exception , baik secara langsung maupun tidak langsung.
* Kelas pengecualian dapat didefinisikan yang melakukan apa saja yang dapat dilakukan oleh kelas lain, tetapi biasanya dibuat sederhana, seringkali hanya menawarkan sejumlah atribut yang memungkinkan informasi tentang kesalahan tersebut diekstraksi oleh penangan sebagai pengecualian. 

## Defining Clean-up Actions
* Pernyataan try memiliki klausa opsional lain yang dimaksudkan untuk mendefinisikan tindakan pembersihan yang harus dijalankan dalam semua keadaan.
* Jika ada klausa finally , klausa finally akan dieksekusi sebagai tugas terakhir sebelum pernyataan try selesai. Klausa finally berjalan apakah pernyataan try menghasilkan pengecualian atau tidak.
* Poin-poin berikut membahas kasus yang lebih kompleks ketika pengecualian terjadi:
	1. Jika pengecualian terjadi selama eksekusi klausa try , pengecualian dapat ditangani oleh klausa except . Jika pengecualian tidak ditangani oleh klausa except , pengecualian akan muncul kembali setelah klausa finally telah dieksekusi.
	2. Pengecualian dapat terjadi selama eksekusi klausa except atau yang else . Sekali lagi, pengecualian akan dimunculkan kembali setelah klausa finally telah dieksekusi.
	3. Jika pernyataan try mencapai break , continue atau return pernyataan, klausa finally akan mengeksekusi tepat sebelum break , continue atau return mengeksekusi pernyataan.
	4. Jika klausa finally menyertakan pernyataan return , nilai yang dikembalikan akan menjadi salah satu dari pernyataan return finally klausa, bukan nilai dari pernyataan return klausa try .

## Predefined Clean-up Actions
* Beberapa objek mendefinisikan tindakan pembersihan standar yang harus dilakukan ketika objek tidak lagi diperlukan, terlepas dari apakah operasi menggunakan objek berhasil atau gagal.
* Pernyataan with memungkinkan objek seperti file untuk digunakan dengan cara yang memastikan mereka selalu dibersihkan dengan cepat dan benar.