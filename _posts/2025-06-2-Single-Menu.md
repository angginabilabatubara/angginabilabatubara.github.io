---
layout: post
title: " Single Menu "
---

penjelasan tentang Single Menu
 

 
##  Apa Itu *Single Menu*?

**Single Menu** merujuk pada **menu navigasi tunggal** dalam sebuah website atau aplikasi. Biasanya ini adalah **menu utama (main navigation)** yang tidak bercabang banyak, sederhana, dan mudah diakses pengguna.

### Contoh:

* Menu horisontal di bagian atas halaman seperti: `Home | About | Contact`
* Satu sidebar tetap tanpa submenu tersembunyi
* Tampilan menu tunggal untuk website one-page


Terima kasih! Sekarang kamu sedang membahas **komponen Single Menu** dalam konteks **antarmuka pengguna (UI)**, bukan navigasi. Jadi yang kamu maksud adalah jenis-jenis komponen input **Single Choice dan Multiple Choice** dalam sebuah menu/form. Berikut adalah penjelasan lengkapnya:



## Komponen Single Menu (Pilihan dalam Form)

Komponen **Single Menu** di sini mengacu pada **komponen UI yang digunakan untuk memilih satu atau beberapa opsi** dari kumpulan pilihan. Ini sangat umum digunakan dalam form HTML dan aplikasi.



### a.  **Radio Button (Pilihan Tunggal)**

###  Fungsi:

Memungkinkan **hanya satu pilihan** dari beberapa opsi.

###  Contoh HTML:

```html
<p>Pilih jenis kelamin:</p>
<input type="radio" name="gender" value="male"> Laki-laki<br>
<input type="radio" name="gender" value="female"> Perempuan<br>
<input type="radio" name="gender" value="other"> Lainnya
```

####  Karakteristik:

* Memiliki `name` yang sama agar hanya satu yang bisa dipilih.
* Digunakan saat pengguna **harus memilih satu opsi** dari beberapa.



### b. **Button Choice (Toggle Button / Button Group)**

###  Fungsi:

Menampilkan pilihan seperti tombol biasa, tetapi hanya satu (atau beberapa) yang bisa aktif.

###  Contoh HTML (dengan Bootstrap 5):

```html
<div class="btn-group" role="group">
  <input type="radio" class="btn-check" name="btnradio" id="btn1" autocomplete="off" checked>
  <label class="btn btn-outline-primary" for="btn1">Option 1</label>

  <input type="radio" class="btn-check" name="btnradio" id="btn2" autocomplete="off">
  <label class="btn btn-outline-primary" for="btn2">Option 2</label>

  <input type="radio" class="btn-check" name="btnradio" id="btn3" autocomplete="off">
  <label class="btn btn-outline-primary" for="btn3">Option 3</label>
</div>
```

###  Karakteristik:

* Lebih interaktif dan stylish.
* Berfungsi sama seperti radio button, tapi tampilannya seperti tombol.


### c.  **Checkbox (Pilihan Ganda)**

###  Fungsi:

Memungkinkan pengguna **memilih lebih dari satu opsi**.

###  Contoh HTML:

```html
<p>Pilih hobi kamu:</p>
<input type="checkbox" name="hobby" value="reading"> Membaca<br>
<input type="checkbox" name="hobby" value="music"> Musik<br>
<input type="checkbox" name="hobby" value="sports"> Olahraga
```

###  Karakteristik:

* Cocok untuk data dengan pilihan **lebih dari satu** (multi-choice).
* Tidak harus ada yang dipilih.


### d.  **Combo Box (Drop Down List)**

###  Fungsi:

Memungkinkan pengguna memilih **satu atau beberapa opsi dari menu tarik turun**.

###  Contoh HTML:

```html
<label for="city">Pilih kota:</label>
<select id="city" name="city">
  <option value="jakarta">Jakarta</option>
  <option value="bandung">Bandung</option>
  <option value="surabaya">Surabaya</option>
</select>
```

###  Karakteristik:

* **Hemat ruang** karena hanya satu baris.
* Ideal untuk pilihan yang **banyak**.
* Bisa dibuat multiple jika diperlukan:

```html
<select multiple>
  <option>Item 1</option>
  <option>Item 2</option>
</select>
```


##  Perbandingan Singkat

| Komponen      | Pilihan               | Interaksi | Contoh Kasus             |
| ------------- | ----------------      | --------- | ------------------------ |
| Radio Button  | Satu                  | Klik      | Jenis Kelamin            |
| Toggle Button | Satu                  | Klik      | Pilihan Mode (Grid/List) |
| Checkbox      | Banyak                | Centang   | Hobi, Fitur Produk       |
| Combo Box     | Satu atau banyak      | Dropdown  | Negara, Kota, Kategori   |


##  Kesimpulan

**Single Menu** cocok untuk situs dengan struktur sederhana dan tujuan yang jelas. Dengan desain yang bersih dan navigasi mudah, single menu memperkuat **fokus konten** dan **user experience**.

 