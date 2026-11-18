# LAB 8 WEB - PHP DAN DATABASE MYSQL

## Identitas
- Nama: Daniel Mohammed
- NIM: (312510466)
- Kelas: I251B
- Mata Kuliah: Pemrograman Web

## 1. Persiapan Praktikum

Pada praktikum ini, dilakukan pembuatan aplikasi CRUD sederhana menggunakan PHP dan database MySQL. Aplikasi dibuat menggunakan Visual Studio Code sebagai text editor dan XAMPP sebagai web server.

Sebelum memulai praktikum, Apache dan MySQL dijalankan melalui XAMPP Control Panel.


## 2. Membuat Database

Database dibuat melalui phpMyAdmin dengan nama `latihan1`.

Selanjutnya, dibuat tabel bernama `data_barang` yang digunakan untuk menyimpan informasi barang.

Tabel tersebut memiliki beberapa kolom, yaitu:
- id_barang
- kategori
- nama
- gambar
- harga_beli
- harga_jual
- stok

## 3. Menambahkan Data Barang

Setelah tabel dibuat, dilakukan penambahan beberapa data barang menggunakan perintah SQL INSERT.

Data yang dimasukkan terdiri dari tiga barang elektronik, yaitu:
- HP Samsung Android
- HP Xiaomi Android
- HP OPPO Android

## 4. Membuat Folder Praktikum

Folder praktikum dibuat di dalam direktori `htdocs` dengan nama `lab8_php_database`.

Folder ini digunakan untuk menyimpan seluruh file aplikasi PHP yang dibuat selama praktikum.

## 5. Membuat Koneksi Database

File `koneksi.php` dibuat untuk menghubungkan aplikasi PHP dengan database MySQL.

Pada file ini digunakan fungsi `mysqli_connect()` dengan beberapa informasi, yaitu host, username, password, dan nama database.

Koneksi diuji melalui browser untuk memastikan PHP berhasil terhubung dengan database.

## 6. Menampilkan Data Barang (Read)

File `index.php` dibuat untuk menampilkan seluruh data barang dari database.

Proses pengambilan data menggunakan perintah SQL SELECT dan fungsi `mysqli_query()`.

Data yang berhasil diambil kemudian ditampilkan dalam bentuk tabel HTML yang berisi gambar, nama barang, kategori, harga jual, harga beli, stok, dan aksi.

Pada halaman ini juga terdapat link untuk menambahkan, mengubah, dan menghapus data barang.


## 7. Menambahkan Data (Create)

File `tambah.php` dibuat untuk menambahkan data barang baru ke dalam database.

Halaman ini memiliki form yang berisi:
- Nama Barang
- Kategori
- Harga Jual
- Harga Beli
- Stok
- File Gambar

Data yang dimasukkan melalui form akan diproses menggunakan metode POST dan disimpan ke database menggunakan perintah SQL INSERT.

## 8. Mengubah Data (Update)

File `ubah.php` dibuat untuk mengubah informasi barang yang sudah tersimpan di database.

Data barang diambil berdasarkan ID barang menggunakan perintah SQL SELECT.

Form akan menampilkan data sebelumnya sehingga pengguna dapat mengubah informasi seperti nama barang, kategori, harga, stok, dan gambar.

Setelah tombol Simpan ditekan, perubahan data akan diproses menggunakan perintah SQL UPDATE.



## 9. Menghapus Data (Delete)

File `hapus.php` dibuat untuk menghapus data barang dari database.

Proses penghapusan dilakukan berdasarkan ID barang menggunakan perintah SQL DELETE.

Setelah data berhasil dihapus, halaman akan kembali ke `index.php` dan menampilkan data barang yang tersisa.


## 10. Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat dipahami cara menghubungkan PHP dengan database MySQL serta menerapkan konsep CRUD (Create, Read, Update, Delete).

Melalui praktikum ini, berhasil dibuat aplikasi sederhana untuk mengelola data barang, mulai dari menambahkan, menampilkan, mengubah, hingga menghapus data menggunakan PHP dan MySQL.


##SCREENSHOT

<img width="1920" height="781" alt="image" src="https://github.com/user-attachments/assets/60072508-b7f9-4a4f-af45-e99f280a0758" />

<img width="534" height="519" alt="image" src="https://github.com/user-attachments/assets/6932e5d6-856f-477b-9de5-9622bba58aaa" />

<img width="655" height="515" alt="image" src="https://github.com/user-attachments/assets/b761152d-6712-48c6-b544-d74c8c757eba" />

<img width="1920" height="629" alt="image" src="https://github.com/user-attachments/assets/80ace00b-8701-4155-be2a-145c30675f42" />
