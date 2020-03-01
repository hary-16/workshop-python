# 6. Modul

Modul adalah file yang berisi definisi dan pernyataan Python. Nama file adalah nama modul dengan akhiran .py ditambahkan. Dalam sebuah modul, nama modul (sebagai string) tersedia sebagai nilai variabel global __name__ . Modul dapat berisi pernyataan yang dapat dieksekusi serta definisi fungsi. Pernyataan-pernyataan ini dimaksudkan untuk menginisialisasi modul. Mereka dieksekusi hanya pertama kali nama modul ditemui dalam pernyataan import. 

* Modul Standar  : 
	Python dilengkapi dengan pustaka modul standar, yang dijelaskan dalam dokumen terpisah, Referensi Pustaka Python (“Pustaka Referensi” selanjutnya). Beberapa modul dibangun ke interpreter; ini memberikan akses ke operasi yang bukan bagian dari inti bahasa tetapi tetap dibangun, baik untuk efisiensi atau untuk menyediakan akses ke sistem operasi primitif seperti panggilan sistem. Set modul tersebut adalah opsi konfigurasi yang juga tergantung pada platform yang mendasarinya.
*  Fungsi dir() : 
	Fungsi dir() digunakan untuk mencari tahu nama mana yang didefinisikan oleh modul.
* Package :
	Paket adalah cara penataan namespace modul Python dengan menggunakan "dotted module names".Ketika mengimpor paket, Python mencari melalui direktori di sys.path mencari subdirektori paket.
	