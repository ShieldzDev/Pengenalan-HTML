Berikut materi **Pertemuan 3: Layout Dasar & Semantic HTML** dalam format Markdown dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 3: Layout Dasar & Semantic HTML

## Konsep Layout dalam HTML

Pada pertemuan sebelumnya, kita sudah bisa menampilkan teks, gambar, dan link. Namun, halaman masih belum memiliki struktur yang jelas.

Layout adalah cara menyusun bagian-bagian halaman agar lebih terorganisir, misalnya:

* Bagian atas (header)
* Menu navigasi
* Konten utama
* Footer

Contoh sederhana tanpa struktur yang jelas:

```html
<h1>Website Saya</h1>
<p>Ini adalah menu</p>
<p>Ini adalah konten</p>
<p>Ini adalah footer</p>
```

Struktur seperti ini sulit dikembangkan. Oleh karena itu, HTML menyediakan cara untuk membuat layout yang lebih rapi.

---

## Menggunakan `<div>` untuk Layout

Tag `<div>` adalah elemen umum (non-semantic) yang digunakan untuk mengelompokkan bagian.

Contoh:

```html
<div>
  <h1>Header</h1>
</div>

<div>
  <p>Menu navigasi</p>
</div>

<div>
  <p>Konten utama</p>
</div>

<div>
  <p>Footer</p>
</div>
```

Kita bisa memberi identitas menggunakan atribut:

```html
<div id="header">
  <h1>Website Saya</h1>
</div>

<div id="content">
  <p>Ini adalah konten</p>
</div>
```

Atau menggunakan class:

```html
<div class="container">
  <p>Isi container</p>
</div>
```

---

## Perbedaan `<div>` dan `<span>`

`<div>` dan `<span>` sama-sama digunakan untuk grouping, tetapi memiliki perbedaan:

* `<div>` adalah elemen block (mengambil satu baris penuh)
* `<span>` adalah elemen inline (tidak memulai baris baru)

Contoh:

```html
<div>Ini div pertama</div>
<div>Ini div kedua</div>
```

Akan tampil terpisah.

```html
<p>
  Ini adalah <span>teks</span> dalam satu baris.
</p>
```

---

## Semantic HTML

Semantic HTML adalah penggunaan tag yang memiliki arti (makna) jelas terhadap isi konten.

Beberapa tag semantic:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<footer>`

Dengan semantic HTML, struktur halaman menjadi lebih mudah dipahami oleh developer lain dan juga mesin pencari.

---

## Contoh Layout dengan Semantic HTML

Berikut contoh struktur halaman menggunakan semantic HTML:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Website Semantic</title>
  </head>
  <body>
    <header>
      <h1>Website Saya</h1>
    </header>

    <nav>
      <a href="#">Home</a>
      <a href="#">Tentang</a>
      <a href="#">Kontak</a>
    </nav>

    <main>
      <section>
        <h2>Artikel 1</h2>
        <p>Ini adalah isi artikel pertama.</p>
      </section>

      <section>
        <h2>Artikel 2</h2>
        <p>Ini adalah isi artikel kedua.</p>
      </section>
    </main>

    <footer>
      <p>Copyright 2026</p>
    </footer>
  </body>
</html>
```

---

## Perbandingan Non-Semantic vs Semantic

### Non-Semantic

```html
<div id="header">
  <h1>Website Saya</h1>
</div>

<div id="nav">
  <a href="#">Home</a>
</div>
```

### Semantic

```html
<header>
  <h1>Website Saya</h1>
</header>

<nav>
  <a href="#">Home</a>
</nav>
```

Semantic lebih jelas dan mudah dibaca.

---

## Block Element vs Inline Element

HTML memiliki dua jenis elemen utama:

### Block Element

* Mengambil satu baris penuh
* Contoh:

```html
<div>Block</div>
<p>Paragraf</p>
<h1>Heading</h1>
```

### Inline Element

* Tidak memulai baris baru
* Contoh:

```html
<span>Inline</span>
<a href="#">Link</a>
<b>Tebal</b>
```

Contoh perbandingan:

```html
<p>
  Ini <span>inline</span> dan tetap satu baris.
</p>

<div>Ini block</div>
<div>Ini block lain</div>
```

---

## Contoh Halaman Lengkap dengan Layout

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Layout Website</title>
  </head>
  <body>

    <header>
      <h1>My Website</h1>
      <p>Belajar HTML</p>
    </header>

    <nav>
      <a href="#">Home</a> |
      <a href="#">Artikel</a> |
      <a href="#">Kontak</a>
    </nav>

    <main>
      <section>
        <h2>Artikel Pertama</h2>
        <p>Ini adalah isi artikel pertama.</p>
      </section>

      <section>
        <h2>Artikel Kedua</h2>
        <p>Ini adalah isi artikel kedua.</p>
      </section>
    </main>

    <footer>
      <p>© 2026 My Website</p>
    </footer>

  </body>
</html>
```

---

## Latihan

Buat halaman HTML dengan struktur:

* Header berisi judul website
* Navigation berisi minimal 3 link
* Main berisi 2 section
* Footer berisi copyright

Gunakan:

* Minimal 2 semantic tag
* Kombinasi `<div>` atau `<span>` jika diperlukan

Contoh kerangka:

```html
<header>...</header>
<nav>...</nav>
<main>
  <section>...</section>
</main>
<footer>...</footer>
```

---
