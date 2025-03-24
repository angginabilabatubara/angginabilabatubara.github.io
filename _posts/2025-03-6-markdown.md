---
layout: post
title: "Markdown"
---

Penjelasan tentang Markdorn

![HTML link dan lists](/assets/images/11zon_resized (3).jpg)

Sumber :revoupedia

## Markdown 

**Markdown** adalah bahasa markup ringan yang digunakan untuk memformat teks dalam bentuk yang mudah dibaca dan ditulis. Markdown dirancang untuk memungkinkan penulisan teks dengan cara yang lebih sederhana dibandingkan dengan HTML, tetapi tetap dapat menghasilkan konten yang terformat dengan baik, seperti heading, daftar, link, gambar, dan lain-lain.

Markdown banyak digunakan di platform blogging, dokumentasi, dan pengelolaan konten karena kesederhanaannya, termasuk di platform seperti **GitHub**, **Jekyll**, dan banyak lainnya.

## Fitur-fitur Utama dalam Markdown

Berikut adalah beberapa fitur umum dan cara penggunaannya dalam Markdown:

#### 1. **Heading (Judul)**
Untuk membuat judul atau heading, kamu bisa menggunakan tanda pagar (`#`). Semakin banyak tanda pagar, semakin rendah tingkat heading-nya.

- `# Heading 1`
- `## Heading 2`
- `### Heading 3`
- `#### Heading 4`
- `##### Heading 5`
- `###### Heading 6`

Contoh:
```markdown
# Judul Utama
## Subjudul
### Sub-subjudul
```

#### 2. **Teks Tebal dan Miring**
- Untuk membuat teks **tebal**, gunakan dua tanda bintang atau garis bawah di kedua sisi kata: `**teks tebal**` atau `__teks tebal__`.
- Untuk membuat teks *miring*, gunakan satu tanda bintang atau garis bawah: `*teks miring*` atau `_teks miring_`.

Contoh:
```markdown
**Teks Tebal**
*TeX Miring*
```

#### 3. **Daftar (List)**

- **Daftar Tidak Terurut**: Gunakan tanda bintang (`*`), tanda tambah (`+`), atau tanda minus (`-`).
  
  Contoh:
  markdown
  - Item 1
  - Item 2
    - Sub-item 1
    - Sub-item 2
  

- **Daftar Terurut**: Gunakan angka diikuti dengan titik (misalnya `1.`, `2.`, dst.)

  Contoh:
  ```markdown
  1. Item pertama
  2. Item kedua
     1. Sub-item pertama
     2. Sub-item kedua
  ```

#### 4. **Tautan (Links)**

Untuk membuat tautan, gunakan format berikut:
```markdown
[teks link](URL)
```

Contoh:
```markdown
[Google](https://www.google.com)
```

#### 5. **Gambar**
Untuk menyisipkan gambar, sintaksnya mirip dengan tautan, tetapi diawali dengan tanda seru (`!`):
```markdown
![alt text](URL gambar)
```

Contoh:
```markdown
![Logo GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
```

#### 6. **Kode (Code)**

- **Kode Inline**: Gunakan satu backtick (`\``) untuk menandai kode dalam teks.
  
  Contoh:
  ```markdown
  `print("Hello World")`
  ```

- **Blok Kode**: Gunakan tiga backticks (```) sebelum dan setelah kode untuk membuat blok kode.
  
  Contoh:
  ```markdown
  ```
  def hello_world():
      print("Hello World")
  ```
  ```

#### 7. **Blockquote (Kutipan)**
Untuk membuat kutipan, gunakan tanda lebih besar (`>`) di awal baris:
```markdown
> Ini adalah kutipan.
```

#### 8. **Horizontal Line (Garis Horizontal)**
Untuk membuat garis horizontal, cukup gunakan tiga tanda minus (`---`), tanda bintang (`***`), atau tanda garis bawah (`___`):
```markdown
---
```

#### 9. **Tabel**
Markdown juga mendukung pembuatan tabel. Sintaks untuk membuat tabel adalah dengan menggunakan tanda pipe (`|`) dan tanda minus (`-`) untuk mendefinisikan baris dan kolom.

Contoh:
```markdown
| Kolom 1 | Kolom 2 | Kolom 3 |
|---------|---------|---------|
| Data 1  | Data 2  | Data 3  |
| Data 4  | Data 5  | Data 6  |
```

---

## Kelebihan Markdown
- **Mudah Dibaca dan Ditulis**: Markdown dirancang untuk dapat dibaca tanpa perlu mengeksekusi kode atau mengubah formatnya. Ini menjadikannya pilihan populer untuk penulisan konten.
- **Portabilitas**: Markdown dapat dengan mudah dikonversi ke format lain seperti HTML, PDF, dan lain-lain.
- **Kompatibilitas**: Markdown digunakan di banyak platform, termasuk GitHub, Jekyll, dan sistem manajemen konten lainnya.

## Penggunaan Markdown di GitHub dan Jekyll
- **GitHub**: Di GitHub, Markdown digunakan untuk membuat file `README.md` yang menjelaskan proyek atau dokumentasi lainnya.
- **Jekyll**: Di Jekyll, file Markdown (`.md`) digunakan untuk membuat halaman statis dan posting blog. Ketika Jekyll membangun situs, file `.md` dikonversi menjadi HTML.

## Contoh Penggunaan Markdown di Jekyll

Misalnya, jika kamu ingin membuat postingan blog di Jekyll, kamu bisa membuat file di folder `_posts` dengan format nama file seperti `2025-03-22-first-post.md`. Isi file tersebut bisa menggunakan sintaks Markdown.

Contoh file `2025-03-22-first-post.md`:
```markdown
---
layout: post
title: "Posting Pertama"
date: 2025-03-22
categories: jekyll update
---

Ini adalah posting pertama saya di Jekyll! Berikut adalah beberapa format Markdown yang saya gunakan.

## Heading 2
Ini adalah teks biasa dengan **teks tebal** dan *teks miring*.

- Item pertama
- Item kedua

[Google](https://www.google.com)
```

Setelah Jekyll membangunnya, file ini akan dikonversi menjadi HTML yang dapat dilihat di situs web.

---

Markdown adalah cara yang cepat dan efisien untuk menulis konten terformat tanpa memerlukan banyak sintaks rumit, menjadikannya pilihan populer di dunia web.
