---
layout: post
title: "Instalasi Ruby dan Jekyll"
---
Penjelasan tentang Instalasi Ruby dan Jekyll

![HTML link dan lists](/assets/images/11zon_resized (3).jpg)

Sumber :revoupedia

Berikut adalah panduan lengkap untuk instalasi dan konfigurasi Jekyll dengan GitHub Pages:

## Instalasi 

#### 1.**Instalasi Ruby**

Ruby adalah bahasa pemrograman yang digunakan oleh Jekyll. Berikut adalah langkah-langkah untuk menginstalnya:

   1. Unduh Ruby Installer:
   - Kunjungi [RubyInstaller for Windows](https://rubyinstaller.org/).
   - Pilih versi Ruby terbaru yang tersedia dan unduh file `.exe`.
   
   2. Jalankan Installer:
   - Setelah diunduh, jalankan installer Ruby dan pastikan untuk mencentang opsi "Add Ruby executables to your PATH".
   - Ikuti langkah-langkah hingga instalasi selesai.

 2.**Instalasi Jekyll**

Setelah Ruby terinstal, langkah selanjutnya adalah menginstal Jekyll dan Bundler (untuk mengelola dependensi Ruby).

  a. Menginstal Jekyll dan Bundler

Instal Bundler:
   - Bundler digunakan untuk mengelola dependensi Ruby. Instal Bundler terlebih dahulu dengan perintah:
     ```
     gem install bundler
     ```
Instal Jekyll:
   - Setelah Bundler terinstal, kamu bisa menginstal Jekyll dengan menjalankan perintah:
     ```
     gem install jekyll
     ```

 b. Verifikasi Instalasi Jekyll

Untuk memastikan bahwa Jekyll terinstal dengan benar, jalankan perintah berikut:
```
jekyll -v
```
Jika instalasi berhasil, kamu akan melihat versi Jekyll yang terinstal.

---
## konfigurasi Jekyll dengan GitHub Pages

Berikut adalah panduan untuk membuat **Personal Web** menggunakan **Jekyll** dan **GitHub Pages**:

#### 1. Membuat Repository GitHub

Untuk meng-host situs Jekyll menggunakan GitHub Pages, kamu perlu membuat repository di GitHub. Ikuti langkah-langkah ini:

1. *Buat Repository Baru di GitHub*:
   - Masuk ke [GitHub](https://github.com/).
   - Klik tombol *New* untuk membuat repository baru.
   - Beri nama repository dengan format username.github.io, misalnya anggi.github.io. Ini adalah nama domain untuk situsmu.
   - Pilih *public* dan jangan centang opsi untuk menambahkan README.
   - Klik *Create repository*.

2. *Salin URL Repository*:
   Salin URL repository GitHub kamu, misalnya:
   
   https://github.com/username/username.github.io
   

#### 2. Membuat Situs Jekyll Baru

Setelah repository GitHub dibuat, langkah berikutnya adalah membuat situs Jekyll secara lokal di komputer kamu.

1. *Buat Situs Jekyll Baru*:
   Di terminal/command prompt, jalankan perintah berikut untuk membuat situs Jekyll baru:
   
   jekyll new nama-repository
   
   Gantilah nama-repository dengan nama yang sesuai. Pastikan folder situsmu sesuai dengan nama repository GitHub kamu nanti.

2. *Pindah ke Direktori Situs*:
   Masuk ke folder situs Jekyll yang baru saja dibuat:
   
   cd nama-repository
   

3. *Verifikasi Situs Secara Lokal*:
   Jalankan situs secara lokal dengan perintah:
   
   bundle exec jekyll serve
   
   Situs akan berjalan di http://localhost:4000. Buka di browser untuk memastikan situs bisa ditampilkan.

#### 3. Menyambungkan Repository GitHub

Sekarang, kita akan menyambungkan situs Jekyll yang baru dibuat ke repository GitHub agar bisa di-hosting di GitHub Pages.

1. *Inisialisasi Git di Direktori Situs*:
   Jika belum, inisialisasi Git di folder situs Jekyll:
   
   git init
   

2. *Hubungkan Repository GitHub*:
   Menambahkan repository GitHub yang baru kamu buat sebagai remote:
   
   git remote add origin https://github.com/username/username.github.io.git
   

3. *Menambahkan dan Meng-commit File*:
   Tambahkan semua file ke staging area dan commit perubahan:
   
   git add .
   git commit -m "Initial commit"
   

4. *Push ke GitHub*:
   Kirimkan file yang sudah di-commit ke GitHub:
   
   git push -u origin main
   
   Jika kamu menggunakan branch master, gunakan perintah ini:
   
   git push -u origin master
   

#### 4. Mengaktifkan GitHub Pages

Sekarang GitHub Pages harus diaktifkan untuk repository kamu.

1. *Masuk ke Pengaturan Repository di GitHub*:
   - Buka halaman repository kamu di GitHub.
   - Klik tab *Settings* di bagian atas halaman.

2. *Aktifkan GitHub Pages*:
   - Di menu *Pages* (bagian bawah kiri), pilih *Source* dan pilih *main branch* (atau master jika kamu menggunakan branch itu).
   - Klik *Save*.

3. *Selesai!*:
   GitHub akan memproses dan meng-host situs Jekyll kamu. Biasanya, situs akan tersedia di:
   
   https://username.github.io
   

#### 5. Menyesuaikan Situs Jekyll

Sekarang situs kamu sudah aktif, kamu bisa menyesuaikan situs dengan mengedit beberapa file.

1. *Konfigurasi _config.yml*:
   Buka file _config.yml dan sesuaikan pengaturan situsmu, seperti nama, deskripsi, dan URL:
   
   title: My Personal Web.

   description: This is my personal website hosted on GitHub Pages.

   url: "https://username.github.io".

   baseurl: "".
   

2. *Menambahkan Postingan Blog atau Halaman Statis*:
   - Untuk menambahkan postingan blog, buat file Markdown di folder _posts dengan format nama YYYY-MM-DD-nama-post.md.
   - Untuk halaman statis seperti "Tentang Saya" atau "Kontak", buat file .md di direktori root situs, misalnya about.md.

3. *Menambahkan Tema Jekyll*:
   Kamu bisa memilih tema dari [Jekyll Themes](https://jekyllrb.com/docs/themes/), lalu menambahkannya ke file _config.yml. Contoh:
   yaml
   theme: jekyll-theme-cayman
   

4. *Menambahkan Custom CSS dan JavaScript*:
   Kamu juga bisa menambahkan file CSS atau JavaScript untuk memperindah tampilan situs di folder assets/css dan assets/js.

#### 6. Update Situs dan Push ke GitHub

Setelah melakukan perubahan pada situs, seperti menambahkan postingan atau mengubah tema, kamu bisa memperbarui situs di GitHub.

1. *Tambah dan Commit Perubahan*:
   Setelah melakukan perubahan, jalankan perintah:
   
   git add .

   git commit -m "Update site content"
   

2. *Push Perubahan ke GitHub*:
   Kirimkan perubahan yang baru saja di-commit ke GitHub:
   
   git push origin main