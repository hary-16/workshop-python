# 12 Virtual Environments and Packages

## 12.1 Introduction
	* Satu instalasi Python tidak mungkin untuk memenuhi persyaratan setiap aplikasi.Solusi untuk masalah ini adalah membuat lingkungan virtual , pohon direktori mandiri yang berisi instalasi Python untuk versi tertentu dari Python, ditambah sejumlah paket tambahan.
## 12.2 Creating Virtual Environments
	* Modul yang digunakan untuk membuat dan mengelola lingkungan virtual disebut venv. venv biasanya akan menginstal versi Python terbaru yang dimiliki. Jika memiliki beberapa versi Python di sistem , dapat memilih versi Python tertentu dengan menjalankan python3atau versi mana pun yang diinginkan.
## 12.3 Managing Packages with pip
	* Untuk menginstal, memutakhirkan, dan menghapus paket dapat menggunakan program yang disebut pip.
	* Secara default pipakan menginstal paket dari Indeks Paket Python, < https://pypi.org > Untuk menelusuri paket python dapat menggunakan browser atau pip search secara terbatas.
	
# Getting started with conda
	Conda adalah manajer paket yang kuat dan manajer lingkungan yang  gunakan dengan perintah baris perintah di Anaconda Prompt untuk Windows, atau di jendela terminal untuk macOS atau Linux.
## Starting conda	
	* Dari menu Start, cari dan buka "Anaconda Prompt."
## Managing conda
	* Untuk melihat versi yang telah di install dengan mengetik conda --version
	* untuk memperbarui versi conda dengan mengetik conda update conda
## Managing environments
	* Conda memungkinkan  untuk membuat lingkungan terpisah yang berisi file, paket, dan dependensinya yang tidak akan berinteraksi dengan lingkungan lain.
	* Ketika mulai menggunakan conda, sudah memiliki lingkungan default bernama base. Saat tidak ingin memasukkan program ke lingkungan basis . Buat lingkungan terpisah untuk menjaga program terisolasi satu sama lain.
## Managing Python
	* Saat membuat lingkungan baru, dapat menginstal versi Python yang sama dengan yang digunakan saat mengunduh dan menginstal Anaconda. Jika ingin menggunakan versi Python yang berbeda, misalnya Python 3.5, cukup buat lingkungan baru dan tentukan versi Python yang diinginkan.
## Managing packages
	* Untuk menemukan paket yang telah diinstal, pertama-tama aktifkan lingkungan yang ingin dicari.
	* Periksa untuk melihat apakah paket yang belum di install bernama "beautifulsoup4" tersedia dari repositori Anaconda.
	* Instal paket ini ke lingkungan saat ini
	* Melihat program baru yang telah di install dengan perintah conda list