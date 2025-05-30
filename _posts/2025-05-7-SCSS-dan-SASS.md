---
layout: post
title: " SCSS dan SASS "
---

penjelasan tentang SCSS dan SASS

SCSS dan SASS adalah **preprocessor CSS**—alat bantu yang memperluas fungsionalitas CSS dan membuat penulisan kode CSS lebih efisien, terstruktur, dan mudah dikelola. Keduanya merupakan bagian dari **Sass (Syntactically Awesome Stylesheets)**, tetapi memiliki perbedaan utama dalam **sintaksis**.

---

##  Apa itu SASS?

**SASS** adalah singkatan dari **Syntactically Awesome Stylesheets**. Ini adalah preprocessor CSS yang menyediakan fitur tambahan seperti:

* Variabel
* Nested rules (aturan bersarang)
* Mixins
* Inheritance
* Modularisasi

### Contoh sintaks SASS (indentasi, tanpa tanda kurung atau titik koma):

```sass
$primary-color: #3498db

body
  background: $primary-color

nav
  ul
    margin: 0
    padding: 0
  li
    display: inline-block
```

---

## Apa itu SCSS?

**SCSS** adalah versi **SASS** yang lebih modern dan menggunakan sintaks seperti **CSS biasa**. Ini adalah bentuk **superset dari CSS**, artinya kode CSS yang valid juga merupakan kode SCSS yang valid.

### Contoh sintaks SCSS (menggunakan `{}` dan `;` seperti CSS):

```scss
$primary-color: #3498db;

body {
  background: $primary-color;
}

nav {
  ul {
    margin: 0;
    padding: 0;
  }

  li {
    display: inline-block;
  }
}
```


##  Kelebihan SCSS/SASS dibanding CSS biasa:

* **Variabel**: menyimpan warna, ukuran, dll.
* **Nesting**: menulis kode hierarki seperti struktur HTML.
* **Partials & Import**: modularisasi file CSS.
* **Mixins & Functions**: reusable styles dengan parameter.
* **Inheritance (`@extend`)**: berbagi style antar selector.

---

##  Kesimpulan

* **SASS** dan **SCSS** adalah alat yang sama dengan dua sintaks berbeda.
* **SCSS lebih populer** karena sintaksnya mirip dengan CSS biasa.
* Keduanya meningkatkan produktivitas dan manajemen proyek front-end.
 
