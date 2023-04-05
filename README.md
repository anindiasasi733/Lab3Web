# Lab3Web
## Profil
| #               | Biodata           |
| --------------- | ----------------- |
| **Nama**        | Anindia Sasikirana|
| **NIM**         | 312110268         |
| **Kelas**       | TI.21.A.2         |
| **Mata Kuliah** | Pemrograman Web 2 |


## Langkah-langkah Praktikum
### Persiapan
Untuk memulai membuat aplikasi CRUD sederhana, yang perlu disiapkan adalah database server
menggunakan MySQL. Pastikan MySQL Server sudah dapat dijalankan melalui XAMPP.<p>
### Menjalankan MySQL Server
Untuk menjalankan MySQL Server dari menu XAMPP Contol.<p>
![Gambar 1](gambar/1.png)
### Mengakses MySQL Client menggunakan PHP MyAdmin
Pastikan webserver Apache dan MySQL server sudah dijalankan. Kemudian buka melalui browser:
http://localhost/phpmyadmin/<p>
### Membuat Database: Studi Kasus Data Barang
![Gambar 2](gambar/2.png)
![Gambar 3](gambar/3.png)
![Gambar 4](gambar/4.png)
![Gambar 5](gambar/5.png)
![Gambar 6](gambar/6.png)

Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL:
http://localhost/lab3_php_database/ <p>
![Gambar 7](gambar/7.png)
### Membuat file koneksi database
Buat file baru dengan nama koneksi.php<p>
```
<?php
$host = "localhost";
$user = "root";
$pass = "";
$db = "latihan1";
$conn = mysqli_connect($host, $user, $pass, $db);
if ($conn == false)
{
echo "Koneksi ke server gagal.";
die();
} #else echo "Koneksi berhasil";
?>
```
Buka melalui browser untuk menguji koneksi database (untuk menyampilkan pesan koneksi berhasil,
uncomment pada perintah echo “koneksi berhasil”;<p>
![Gambar 8](gambar/8.png)
### Membuat file index untuk menampilkan data (Read)
