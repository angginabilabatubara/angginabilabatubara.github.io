---
layout: post
title: " Dasar PHP "
---

penjelasan tentang  Dasar PHP




##  Apa Itu PHP?

**PHP (Hypertext Preprocessor)** adalah bahasa pemrograman **server-side** yang dirancang untuk membuat halaman web dinamis. Artinya, PHP berjalan di server dan hasilnya dikirimkan ke browser dalam bentuk HTML.

PHP digunakan untuk:

* Memproses formulir HTML
* Mengakses database (seperti MySQL)
* Membuat sistem login
* Mengelola file
* Dan banyak lagi
 

##  Cara Menjalankan PHP

Karena PHP berjalan di server, kamu butuh:

1. **Web Server** seperti Apache
2. **PHP Interpreter**
3. **Database** (opsional) seperti MySQL

Cara termudah adalah dengan menginstal **XAMPP** atau **Laragon**:

* [Download XAMPP](https://www.apachefriends.org/)
* Simpan file PHP di folder `htdocs`
* Akses lewat browser: `http://localhost/namafile.php`



##  Struktur File Dasar PHP

File PHP memiliki ekstensi **`.php`**. Contoh:

```php
<!-- hello.php -->
<?php
  echo "Halo, dunia!";
?>
```

Ketika dibuka di browser melalui `localhost`, maka akan tampil:
`Halo, dunia!`


##  Dasar-Dasar Sintaks PHP

### 1. **Tag Pembuka PHP**

```php
<?php
// Kode PHP ditulis di sini
?>
```

### 2. **Output**

```php
echo "Teks yang dicetak";
print "Ini juga mencetak teks";
```

### 3. **Variabel**

```php
$nama = "Anggi";
$umur = 20;

echo "Halo, nama saya $nama dan umur saya $umur tahun.";
```

### 4. **Tipe Data**

* String: `"teks"`
* Integer: `1, 10, -5`
* Float: `3.14`
* Boolean: `true`, `false`
* Array: `["apel", "jeruk"]`
* Object: (nanti dipelajari di OOP)

 

##  Operator dan Percabangan

### 1. **Operator Aritmatika**

```php
$a = 5;
$b = 2;

echo $a + $b;  // Hasil: 7
echo $a * $b;  // Hasil: 10
```

### 2. **Percabangan If**

```php
$nilai = 75;

if ($nilai >= 80) {
  echo "Nilai A";
} elseif ($nilai >= 70) {
  echo "Nilai B";
} else {
  echo "Nilai C";
}
```

 

##  Perulangan (Looping)

### 1. **For**

```php
for ($i = 1; $i <= 5; $i++) {
  echo "Angka: $i <br>";
}
```

### 2. **While**

```php
$i = 1;
while ($i <= 3) {
  echo "Baris ke-$i <br>";
  $i++;
}
```

 

##  Form dan $\_GET / $\_POST

### Form HTML + PHP

```html
<form action="proses.php" method="post">
  Nama: <input type="text" name="nama">
  <input type="submit" value="Kirim">
</form>
```

### File `proses.php`

```php
<?php
$nama = $_POST['nama'];
echo "Halo, $nama!";
?>
```

 

##  Array

```php
$buah = ["apel", "mangga", "jeruk"];
echo $buah[1]; // mangga

foreach ($buah as $item) {
  echo $item . "<br>";
}
```

 

##  Mengakses Database MySQL

### 1. Koneksi Database

```php
$conn = mysqli_connect("localhost", "root", "", "nama_database");

if (!$conn) {
  die("Koneksi gagal: " . mysqli_connect_error());
}
```

### 2. Menampilkan Data

```php
$result = mysqli_query($conn, "SELECT * FROM mahasiswa");

while ($row = mysqli_fetch_assoc($result)) {
  echo $row['nama'] . "<br>";
}
```

 

##  Fungsi PHP

```php
function sapa($nama) {
  return "Halo, $nama!";
}

echo sapa("Alya");
```

 

## 📦 File dan Include

```php
// file: header.php
echo "<h1>Header Website</h1>";

// file utama:
include 'header.php';
```

 

## Fitur Tambahan (lanjutan)

* Session & Cookie
* Upload File
* Validasi Form
* Login & Register
* OOP (Pemrograman Berorientasi Objek)
 
##  Kesimpulan

PHP adalah bahasa yang **mudah dipelajari**, **berkembang pesat**, dan **digunakan secara luas** di pengembangan web. Jika kamu ingin membuat website dinamis, memahami PHP adalah **langkah awal yang sangat bagus**.

 