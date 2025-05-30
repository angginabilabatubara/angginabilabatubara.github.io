---
layout: post
title: "Config.yml"
---


Penjelasan tentang Config.yml

##  Apa itu `_config.yml` di Jekyll?

`_config.yml` adalah file konfigurasi utama dalam proyek Jekyll, yaitu platform pembuat situs statis berbasis Ruby. File ini digunakan untuk mengatur hampir semua aspek situs statis kamu, seperti:

* Nama blog atau situs
* Deskripsi
* Tema yang digunakan
* Plugin
* Struktur URL
* Metadata penulis, dll.

---

Baik, Anggi Syaban Nabila! Berikut ini versi revisi dari penjelasan lengkap tentang `_config.yml` Jekyll yang menggunakan namamu sebagai contoh di dalam kontennya:

---

##  Apa Itu `_config.yml`?

File `_config.yml` adalah **jantung pengaturan** dalam proyek Jekyll. Semua konfigurasi utama situs kamu — seperti nama situs, deskripsi, URL, hingga plugin yang digunakan — diatur melalui file ini. Jekyll akan membaca file ini setiap kali kamu membangun (build) situs statis.

Karena menggunakan format **YAML**, file ini sangat mudah dibaca dan ditulis. Formatnya sederhana, namun fleksibel untuk berbagai kebutuhan.

---

##  Lokasi File

File `_config.yml` diletakkan di **root direktori proyek Jekyll**, bersama file seperti `index.md` dan folder `_posts/`.

---

##  Struktur Dasar `_config.yml`

Contoh pengaturan awal untuk blog pribadi milik Anggi:

```yaml
title: Anggi Syaban Nabila's Blog
description: Catatan pribadi dan perjalanan belajar
url: "https://angginabilabatubara.github.io/"
baseurl: "" # kosong jika situs tidak di dalam sub-folder
theme: minima
```

### Penjelasan:

* **`title`**: Nama situs yang akan tampil di browser atau halaman utama.
* **`description`**: Deskripsi singkat untuk SEO dan identitas blog.
* **`url`**: Alamat utama blog kamu di GitHub Pages.
* **`baseurl`**: Diisi jika situs kamu berada dalam subfolder (kosong jika tidak).
* **`theme`**: Tema yang digunakan, seperti `minima`, `jekyll-theme-cayman`, dsb.

---

##  Menambahkan Plugin

Untuk memperluas fitur situs, kamu bisa menambahkan plugin:

```yaml
plugins:
  - jekyll-feed
  - jekyll-seo-tag
```

### Contoh kegunaannya:

* `jekyll-feed`: Menyediakan RSS feed otomatis.
* `jekyll-seo-tag`: Mengelola metadata SEO otomatis.

---

##  Konfigurasi Tambahan

Tambahan konfigurasi yang sering digunakan:

```yaml
author:
  name: Anggi Syaban Nabila
  email: anggisyabannabilaagmail.com

permalink: /:title/
paginate: 5
paginate_path: "/page:num"
markdown: kramdown
highlighter: rouge
```

### Penjelasan:

* **`author`**: Identitas penulis yang bisa ditampilkan di halaman blog.
* **`permalink`**: Struktur URL untuk postingan (misal: `/judul-posting/`).
* **`paginate`**: Jumlah postingan per halaman jika menggunakan pagination.
* **`markdown`**: Mesin konversi Markdown, `kramdown` adalah default Jekyll.
* **`highlighter`**: Untuk menyoroti kode program (`rouge` adalah defaultnya).

---

##  Variabel Kustom

Kamu juga bisa membuat variabel sendiri:

```yaml
social:
  github: https://github.com/anggisyaban
  instagram: https://instagram.com/anggisyaban
```

Lalu dipanggil di layout:

```liquid
<a href="{{ site.social.github }}">GitHub</a>
```

---

##  Mode Build Multi-Konfigurasi

Untuk keperluan produksi dan pengembangan:

```bash
jekyll build --config _config.yml,_config-dev.yml
```

Ini memungkinkan kamu memisahkan konfigurasi untuk testing dan produksi.

---

##  Tips dan Catatan

* YAML sensitif terhadap spasi: gunakan 2 spasi, jangan tab.
* Gunakan `#` untuk komentar.
* Hindari kutip ganda atau kutip tunggal kecuali diperlukan.

---

##  Kesimpulan

File `_config.yml` memudahkan kamu mengelola blog statis Jekyll secara fleksibel dan efisien. Dengan satu file ini, kamu bisa mengatur tampilan, metadata, struktur URL, plugin, hingga info pribadi seperti nama dan akun media sosial.

Jadi, bagi kamu yang sedang membangun blog dengan Jekyll seperti Anggi Syaban Nabila, memahami `_config.yml` adalah langkah awal untuk membentuk situs pribadi yang rapi, terstruktur, dan profesional.
 n