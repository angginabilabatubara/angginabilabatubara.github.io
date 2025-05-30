---
layout: post
title: " Formspree "
---

penjelasan tentang Formspree
 


 
## **Apa itu Formspree**
Formspree adalah layanan pihak ketiga berbasis web yang memungkinkan pengembang dan desainer web menghubungkan formulir HTML di website mereka dengan alamat email tanpa memerlukan kode backend (seperti PHP, Node.js, Python, dsb.).

Dengan Formspree, kamu bisa membuat formulir kontak, formulir pendaftaran, dan berbagai jenis form lainnya yang secara otomatis mengirimkan datanya langsung ke email kamu. Ini sangat berguna terutama bagi:

Pengembang yang menggunakan situs statis (HTML/CSS/JS saja)

Website personal, portofolio, blog

Website yang dihosting di GitHub Pages, Netlify, atau Vercel

Proyek yang tidak memiliki server backend

##  **Tujuan dan Kegunaan Formspree**

Formspree dibuat untuk **menyederhanakan proses pengelolaan formulir di web**, khususnya untuk website yang tidak menggunakan backend. Tujuannya adalah:

* Menghindari kerumitan membuat API atau script PHP
* Memberikan solusi yang cepat dan mudah dipasang
* Menyediakan antarmuka dan keamanan untuk menerima data dari pengguna

Dengan Formspree, kamu bisa:

* Menerima pesan dari formulir kontak
* Mendapat notifikasi email setiap kali form dikirim
* Menganalisis statistik pengisian form
* Mengatur validasi dan keamanan dari serangan spam


##  **Bagaimana Cara Kerja Formspree?**

1. Kamu **membuat form HTML** di halaman web kamu seperti biasa.
2. Kamu **mengubah atribut `action`** pada tag `<form>` menjadi URL endpoint yang diberikan oleh Formspree.
3. Ketika pengunjung mengisi formulir dan mengirimnya:

   * Data akan dikirim ke server Formspree.
   * Formspree akan **memvalidasi** data dan email penerima.
   * Jika valid, **email akan dikirimkan ke kamu** berisi isi form tersebut.
   * Kamu bisa menambahkan opsi redirect ke halaman terima kasih.


## **Contoh Form HTML Sederhana Menggunakan Formspree**

```html
<form action="https://formspree.io/f/mnqyljkd" method="POST">
  <label>Nama:
    <input type="text" name="name" required>
  </label>
  <label>Email:
    <input type="email" name="email" required>
  </label>
  <label>Pesan:
    <textarea name="message" required></textarea>
  </label>
  <button type="submit">Kirim</button>
</form>
```

 URL `https://formspree.io/f/mnqyljkd` adalah endpoint yang kamu dapatkan setelah membuat akun Formspree dan membuat form baru. Ganti dengan URL-mu sendiri.



##  **Fitur-Fitur Utama Formspree**

### 1.  **Pengiriman Data via Email**

Setiap kali formulir dikirim, kamu akan langsung menerima email yang berisi informasi dari form pengguna.

### 2.  **Validasi Otomatis**

Formspree mendukung validasi HTML5 (seperti `required`, `email`) dan bisa ditambahkan validator di sisi server.

### 3.  **Redirect Setelah Submit**

Kamu bisa mengatur agar setelah pengguna mengisi form, mereka akan diarahkan ke halaman tertentu, misalnya `thank-you.html`.

```html
<input type="hidden" name="_redirect" value="https://namadomainmu.com/terima-kasih.html">
```

### 4.  **Proteksi Spam**

* Mendukung honeypot (form tersembunyi untuk mendeteksi bot)
* Mendukung Google reCAPTCHA (pada versi Pro)
* Pembatasan IP jika diperlukan

### 5.  **Custom Email Template**

Kamu bisa mengatur seperti apa email yang dikirim ke kamu—menyesuaikan dengan kebutuhan.

### 6.  **Analytics dan Statistik**

Fitur ini tersedia di versi Pro, memungkinkan kamu melihat performa form: berapa kali dikirim, IP pengirim, waktu pengiriman, dsb.

### 7.  **Integrasi API & Webhook**

Kamu bisa mengirim data form langsung ke Slack, Zapier, Google Sheets, atau layanan backend melalui webhook.
 

##  **Langkah-Langkah Menggunakan Formspree**

1. Daftar akun di [https://formspree.io](https://formspree.io)
2. Buat project dan form baru (akan diberikan link endpoint)
3.Salin link endpoint an gunakan pada atribut `action` di form HTML kamu
4. Pasang validasi tambahan (opsional)
5. Coba kirim form dan cek email
6. Tambahkan redirect atau pesan sukses sesuai kebutuhan
7. (Opsional) **Integrasikan reCAPTCHA atau webhook**

 

##  **Tips Penggunaan Formspree yang Efektif**

* Gunakan **validasi HTML5** seperti `required`, `pattern`, `type=email`, dll.
* Tambahkan **honeypot** field tersembunyi untuk menangkal spam bot.
* Tambahkan **`_replyto`** untuk membalas langsung ke pengirim melalui email.

  ```html
  <input type="email" name="_replyto">
  ```
* Buat halaman `terima-kasih.html` sebagai redirect setelah pengiriman sukses.

##  **Contoh Form Lebih Lengkap**

```html
<form action="https://formspree.io/f/mnqyljkd" method="POST">
  <label>Nama Lengkap:
    <input type="text" name="nama" required>
  </label>
  <label>Email Aktif:
    <input type="email" name="_replyto" required>
  </label>
  <label>Topik:
    <select name="topik">
      <option value="dukungan">Dukungan</option>
      <option value="kritik">Kritik</option>
      <option value="saran">Saran</option>
    </select>
  </label>
  <label>Pesan:
    <textarea name="pesan" required></textarea>
  </label>
  <input type="hidden" name="_subject" value="Pesan dari Website!">
  <input type="hidden" name="_redirect" value="https://domainkamu.com/terima-kasih.html">
  <button type="submit">Kirim Sekarang</button>
</form>
```


##  **Dokumentasi dan Bantuan**

* Situs Resmi: [https://formspree.io](https://formspree.io)
* Dokumentasi lengkap: [https://formspree.io/docs](https://formspree.io/docs)
* GitHub repository: [https://github.com/formspree/formspree](https://github.com/formspree/formspree)
* Dukungan email & komunitas tersedia untuk pengguna Pro


##  **Kesimpulan**

**Formspree** adalah solusi modern dan praktis untuk mengelola formulir web tanpa backend. Sangat cocok bagi pengguna situs statis atau pengembang yang tidak ingin repot mengatur server. Dengan fitur seperti email otomatis, redirect, validasi, dan integrasi API/webhook, Formspree menjadikan pengelolaan form menjadi cepat, aman, dan profesional.

 
 
