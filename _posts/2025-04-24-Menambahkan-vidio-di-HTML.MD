---
layout: post
title: "Menambahkan vidio di HTML"
---
Penjelasan tentang menambahkan vidio

 

##  Cara menambahkan video di HTML

HTML menyediakan elemen `<video>` untuk menyisipkan dan memutar video secara langsung di halaman web.

###  Struktur Dasar:

```html
<video controls>
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```


##  Penjelasan setiap bagian

| Bagian        | Fungsi                                                     |
| ------------- | ---------------------------------------------------------- |
| `<video>`     | Elemen utama untuk memutar video                           |
| `controls`    | Menampilkan kontrol play, pause, volume, dll               |
| `<source>`    | Menentukan file video dan formatnya                        |
| `type`        | Memberitahu browser format file video (misal: `video/mp4`) |
| Teks fallback | Akan muncul jika browser tidak mendukung video             |



##  Atribut penting lainnya

| Atribut               | Fungsi                                          |
| --------------------- | ----------------------------------------------- |
| `controls`            | Menampilkan tombol play/pause, dll              |
| `autoplay`            | Video akan langsung diputar saat halaman dibuka |
| `loop`                | Video akan mengulang terus-menerus              |
| `muted`               | Video dimulai dalam keadaan tanpa suara         |
| `poster="gambar.jpg"` | Gambar thumbnail sebelum video diputar          |
| `width="600"`         | Menentukan lebar video (dalam piksel)           |


##  contoh lengkap:

```html
<video width="600" controls autoplay loop muted poster="thumbnail.jpg">
  <source src="video-keren.mp4" type="video/mp4">
  <source src="video-keren.webm" type="video/webm">
  Browser Anda tidak mendukung pemutar video HTML5.
</video>
```


## Menyematkan Video dari Youtube (Embed)

Jika videonya berasal dari YouTube:

```html
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/VIDEO_ID" 
  title="YouTube video player" 
  frameborder="0" 
  allowfullscreen>
</iframe>
```

> Gantilah `VIDEO_ID` dengan ID video asli dari YouTube (misalnya: `dQw4w9WgXcQ`).


##  Catatan 

* Format video yang paling umum dan didukung luas adalah `.mp4`
* File video sebaiknya berada di folder proyek atau dihosting secara online
* Gunakan lebih dari satu format (`.mp4`, `.webm`, dll) jika ingin kompatibilitas maksimal

 