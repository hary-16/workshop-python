# 10 Perpustakaan Standar

## 10.1 Operating System Interface
	* Dengan OS modul,menyediakan puluhan fungi untuk berinteraksi dengan sistem operasi.
## 10.2 File Wildcards
	* Modul glob menyediakan fungsi untuk membuat daftar file dari pencarian direktori wildcard.
## 10.3 Command Line Arguments
	* Skrip utilitas umum seringkali perlu memproses argumen baris perintah. Argumen-argumen ini disimpan dalam atribut argvsys modul sebagai daftar.
	* Modul argparse menyediakan mekanisme yang lebih canggih untuk argumen baris perintah proses.
## 10.4 Error Output Redirection and Program Termination
	* Modul sys juga memiliki atribut untuk stdin , stdout , dan stderr . Yang terakhir berguna untuk memancarkan peringatan dan pesan kesalahan untuk membuatnya terlihat bahkan ketika stdout telah diarahkan.
	* Cara paling langsung untuk mengakhiri skrip adalah dengan menggunakan sys.exit().
## 10.5 String Pattern Matching
	* Modul re menyediakan alat ekspresi reguler untuk pengolahan string yang canggih. Untuk pencocokan dan manipulasi yang kompleks, ekspresi reguler menawarkan solusi yang ringkas dan dioptimalkan.
## 10.6 Mathematics
	* Modul math memberikan akses ke mendasari C fungsi perpustakaan untuk floating point matematika.
	* Modul random menyediakan alat untuk membuat pilihan acak.
	* Modul statistics menghitung sifat statistik dasar (mean, median, varians, dll) dari data numerik.
## 10.7 Internet Access
	* Dua modul yang paling sederhana untuk mengakses internet dan memproses protokol internnet adalah urllib.requestuntuk mengambil data dari URL dan smtplibuntuk mengirim surat.
## 10.8 Dates and Times
	* Modul datetime kelas untuk memanipulasi tanggal dan waktu di kedua sederhana dan cara yang kompleks. Sementara aritmatika tanggal dan waktu didukung, fokus implementasi adalah pada ekstraksi anggota yang efisien untuk pemformatan dan manipulasi output. Modul ini juga mendukung objek yang sadar zona waktu.
## 10.9 Data Compression 
	* Pengarsipan data umum dan kompresi format secara langsung didukung oleh modul termasuk: zlib, gzip, bz2, lzma, zipfiledan tarfile.
## 10.10 Performance Measurement
	* Beberapa pengguna Python mengembangkan minat mendalam untuk mengetahui kinerja relatif dari berbagai pendekatan untuk masalah yang sama. Python menyediakan alat pengukuran yang segera menjawab pertanyaan-pertanyaan itu.
## 10.11 Quality Control 
	* Salah satu pendekatan untuk mengembangkan perangkat lunak berkualitas tinggi adalah dengan menulis tes untuk setiap fungsi saat dikembangkan dan untuk menjalankan tes tersebut sering selama proses pengembangan.
	* Modul doctest menyediakan alat untuk memindai modul dan memvalidasi tes tertanam dalam docstrings program ini. Konstruksi pengujian sesederhana memotong dan menempel panggilan khas beserta hasilnya ke dalam docstring. Ini meningkatkan dokumentasi dengan memberikan contoh kepada pengguna dan memungkinkan modul doctest memastikan kode tetap benar untuk dokumentasi.
	* Modul unittest ini tidak mudah seperti doctest modul, tetapi memungkinkan satu set yang lebih komprehensif dari tes untuk dipertahankan dalam file terpisah.
## 10.12 Batteries Included
	* Python memiliki filosofi "batteries included". Ini paling baik dilihat melalui kemampuan yang canggih dan kuat dari paket-paket yang lebih besar.
	* Modul ***xmlrpc***.*client* dan ***xmlrpc***.***server*** menjadikan penerapan panggilan prosedur jarak jauh menjadi tugas yang hampir sepele. Terlepas dari nama-nama modul, tidak diperlukan pengetahuan atau penanganan XML secara langsung.
	* Paket ***email*** adalah perpustakaan untuk mengelola pesan email, termasuk MIME dan dokumen pesan berbasis **RFC** **2822** lainnya. Tidak seperti **smtplib** dan ***poplib*** yang benar-benar mengirim dan menerima pesan, paket email memiliki perangkat lengkap untuk membangun atau mendekodekan struktur pesan yang kompleks (termasuk lampiran) dan untuk mengimplementasikan pengkodean internet dan protokol header.
	* Paket ***json*** menyediakan dukungan kuat untuk mem-parsing format pertukaran data populer ini. Modul ***csv*** mendukung pembacaan dan penulisan file secara langsung dalam format Nilai Terpisah Koma, yang umumnya didukung oleh database dan spreadsheet. Pemrosesan XML didukung oleh paket ***xml.etree.ElementTree***, ***xml.dom*** dan ***xml.sax***. Bersama-sama, modul dan paket ini sangat menyederhanakan pertukaran data antara aplikasi Python dan alat lainnya.
	* Modul ***sqlite3*** adalah pembungkus untuk pustaka database SQLite, menyediakan database persisten yang dapat diperbarui dan diakses menggunakan sintaks SQL yang sedikit tidak standar.
	* Internasionalisasi didukung oleh sejumlah modul termasuk ***gettext***, ***locale***, dan paket ***codec***.

# Perpustakaan Standar - Bagian II

## 11.1
	* Modul reprlib menyediakan versi repr()disesuaikan untuk menampilkan disingkat kontainer besar atau sangat bersarang
	* Modul pprint kontrol yang lebih canggih lebih mencetak baik built-in dan benda-benda yang ditetapkan pengguna dengan cara yang dapat dibaca oleh interpreter. 
	* Modul textwrap format paragraf teks agar sesuai dengan lebar layar yang diberikan.
	* Modul locale mengakses database format data tertentu budaya. Atribut pengelompokan fungsi format lokal menyediakan cara langsung memformat angka dengan pemisah grup.
## 11.2 Templating
	* Modul string termasuk serbaguna,Kelas Template dengan sintaks disederhanakan cocok untuk mengedit oleh pengguna akhir. Ini memungkinkan pengguna untuk menyesuaikan aplikasi mereka tanpa harus mengubah aplikasi.Format ini menggunakan nama placeholder yang dibentuk oleh $dengan pengidentifikasi Python yang valid
	* Metode substitute() menimbulkan KeyErrorketika pengganti tidak disediakan dalam kamus atau argumen kata kunci. Untuk aplikasi gaya gabungan surat, data yang diberikan pengguna mungkin tidak lengkap dan safe_substitute()metode ini mungkin lebih sesuai - itu akan membuat placeholder tidak berubah jika data hilang.
	* Aplikasi lain untuk templating adalah memisahkan logika program dari detail berbagai format output. Ini memungkinkan untuk mengganti template khusus untuk file XML, laporan teks biasa, dan laporan web HTML.
## 11.3 Working with Binary Data Record Layouts
	* Modul struct menyediakan pack()dan unpack()fungsi untuk bekerja dengan format rekaman biner variabel panjang.
## 11.4 Multi-threading
	* Threading adalah teknik untuk memisahkan tugas-tugas yang tidak tergantung secara berurutan. Threading dapat digunakan untuk meningkatkan responsif aplikasi yang menerima input pengguna saat tugas lain berjalan di latar belakang. Kasus penggunaan terkait menjalankan I / O secara paralel dengan perhitungan di utas lainnya.
	* Modul threading tingkat tinggi dapat menjalankan tugas di latar belakang sementara program utama terus berjalan
	* Tantangan utama aplikasi multi-utas adalah mengoordinasikan utas yang berbagi data atau sumber daya lainnya. Untuk itu, modul threading menyediakan sejumlah primitif sinkronisasi termasuk kunci, peristiwa, variabel kondisi, dan semaphore.
## 11.5 Logging
	* Modul logging menawarkan sistem logging fitur dan fleksibel penuh. Paling sederhana, pesan log dikirim ke file atau ke sys.stderr.
	* Sistem logging dapat dikonfigurasikan secara langsung dari Python atau dapat diambil dari file konfigurasi yang dapat diedit pengguna untuk logging yang dikustomisasi tanpa mengubah aplikasi.
## 11.6 Weak References
	* Python melakukan manajemen memori otomatis (penghitungan referensi untuk sebagian besar objek dan pengumpulan sampah untuk menghilangkan siklus). Memori dibebaskan tidak lama setelah referensi terakhir untuk itu telah dihilangkan.
	* Modul weakref menyediakan alat untuk objek pelacakan tanpa membuat referensi. Ketika objek tidak lagi diperlukan, itu secara otomatis dihapus dari tabel lemahref dan panggilan balik dipicu untuk objek lemah.
## 11.7 Tools for Working with Lists
	* Modul array menyediakan array()objek yang seperti daftar yang menyimpan hanya homogen data dan menyimpannya lebih kompak.
	* Modul collections menyediakan deque()objek yang seperti daftar dengan menambahkan lebih cepat dan muncul dari sisi kiri namun pencarian lebih lambat di tengah. Objek-objek ini sangat cocok untuk mengimplementasikan antrian dan pencarian pohon pertama yang luas.
	* Modul heapq menyediakan fungsi untuk melaksanakan tumpukan berdasarkan daftar reguler. Entri bernilai terendah selalu disimpan di posisi nol. Ini berguna untuk aplikasi yang berulang kali mengakses elemen terkecil tetapi tidak ingin menjalankan pengurutan daftar lengkap.
## 11.8 Decimal Floating Point Arithmetic
	* Modul decimal menawarkan Decimaldatatype untuk desimal aritmatika floating point. Dibandingkan dengan float implementasi built-in floating point biner, kelas ini sangat membantu.
	

