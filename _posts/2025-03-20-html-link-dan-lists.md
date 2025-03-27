---
layout: post
title: "Html link and lists"
---


Penjelasan tentang link dan list pada HTML

![HTML link dan lists](/assets/images/11zon_resized (3).jpg) 

Sumber :revoupedia  

## **1. LINK (`<a>` - Anchor Tag)**
Link dalam HTML digunakan untuk **menghubungkan** satu halaman ke halaman lain, baik dalam situs yang sama maupun ke situs eksternal. Link dibuat dengan elemen `<a>` (**anchor tag**).

---

### **1.1 Struktur Dasar Link**  
```html
<a href="https://www.example.com">Klik di sini</a>
```
🔹 **`href="URL"`** → Menentukan tujuan link (bisa ke halaman lain atau situs luar).  
🔹 **Teks di antara `<a>` dan `</a>`** akan menjadi teks yang bisa diklik.  

---

### **1.2 Jenis-Jenis Link**  

#### **1.2.1 Link ke Halaman Lain**
```html
<a href="halaman-lain.html">Buka Halaman Lain</a>
```
 Menghubungkan halaman dalam situs yang sama.

#### **1.2.2 Link ke Website Luar**
```html
<a href="https://www.google.com">Kunjungi Google</a>
```
 Menghubungkan ke website lain di internet.

#### **1.2.3 Link dengan Target (Membuka di Tab Baru)**
```html
<a href="https://www.google.com" target="_blank">Buka Google di Tab Baru</a>
```
`target="_blank"` membuat link terbuka di tab atau jendela baru.

#### **1.2.4 Link ke Email**
```html
<a href="mailto:email@example.com">Kirim Email</a>
```
 Saat diklik, akan membuka aplikasi email untuk mengirim pesan.

#### **1.2.5 Link ke Nomor WhatsApp**
```html
<a href="https://wa.me/6281234567890">Chat WhatsApp</a>
```
 Menghubungkan langsung ke chat WhatsApp.

#### **1.2.6 Link ke Bagian Tertentu dalam Halaman (Anchor Link)**
```html
<a href="#section2">Loncat ke Bagian 2</a>

<h2 id="section2">Bagian 2</h2>
```
 Klik link ini akan langsung menggulir ke bagian dengan `id="section2"`.

---

## **2. LIST (Daftar dalam HTML)**
List digunakan untuk membuat daftar item, baik dalam bentuk **berurutan (ordered list)** atau **tidak berurutan (unordered list)**.

---

### **2.1 Unordered List (`<ul>`)**
Digunakan untuk daftar **tanpa nomor** (hanya menggunakan bullet/buletan).  

#### **Contoh:**
```html
<ul>
  <li>Apel</li>
  <li>Pisang</li>
  <li>Mangga</li>
</ul>
```
 `<ul>` → Menandakan bahwa ini adalah daftar tidak berurutan.  
 `<li>` → Setiap item daftar ditulis di dalamnya.  

**Hasilnya:**  
- Apel  
- Pisang  
- Mangga  

---

### **2.2 Ordered List (`<ol>`)**
Digunakan untuk daftar **dengan nomor atau urutan**.

#### **Contoh:**
```html
<ol>
  <li>Bangun pagi</li>
  <li>Sarapan</li>
  <li>Berangkat kerja</li>
</ol>
```
 `<ol>` → Menandakan daftar berurutan.  
 `<li>` → Setiap item daftar.  

**Hasilnya:**  
1. Bangun pagi  
2. Sarapan  
3. Berangkat kerja  

 **Mengubah tipe angka dalam `<ol>`:**  
```html
<ol type="A">
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```
 Hasilnya akan menggunakan huruf: **A. Item 1, B. Item 2**.

Tipe `<ol>` lainnya:
- `type="1"` → 1, 2, 3 (default)
- `type="A"` → A, B, C
- `type="a"` → a, b, c
- `type="I"` → I, II, III
- `type="i"` → i, ii, iii

---

### **2.3 Description List (`<dl>`)**
Digunakan untuk membuat daftar dengan **deskripsi/keterangan**.

#### **Contoh:**
```html
<dl>
  <dt>Kucing</dt>
  <dd>Hewan peliharaan yang lucu.</dd>

  <dt>Anjing</dt>
  <dd>Hewan penjaga yang setia.</dd>
</dl>
```
 `<dl>` → Menandakan daftar deskripsi.  
 `<dt>` → Menandai judul item.  
 `<dd>` → Menandai deskripsi dari item.  

**Hasilnya:**  
**Kucing**  
Hewan peliharaan yang lucu.  

**Anjing**  
Hewan penjaga yang setia.  

---

## **Kesimpulan**
### Link (`<a>`):
 Menghubungkan halaman atau situs lain.  
 Bisa ke email, WhatsApp, atau bagian tertentu dalam halaman.  
 Bisa dibuka di tab baru dengan `target="_blank"`.  

###  List (`<ul>`, `<ol>`, `<dl>`):
 **`<ul>`** → Daftar tanpa nomor (bullet points).  
 **`<ol>`** → Daftar dengan nomor (ordered list).  
 **`<dl>`** → Daftar dengan deskripsi.  

---
 